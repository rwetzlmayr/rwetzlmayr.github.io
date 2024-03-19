---
layout: post
title: wet_slimpattern: Integrating SlimStat into Textpattern
---

**wet_slimpattern** is a plugin which integrates [Textpattern](https://textpatttern.com "The small content management system that can handle big ideas") with **SlimStat**, an open source web statistics package developed by Stephen Wettone.

### The Traditional Approach

Typically, the integration of SlimStat into Textpattern is accomplished by modifying the `index.php` file in the root folder of your Textpattern installation to include a call to the hit-logging code provided by SlimStat. This is straightforward and works as it should, but it requires modifying a file that is part of the Textpattern distribution. This small modification could cause issues during upgrades and needs to be tracked.

### The textpatterned way of doing things

As an alternative way to integrate the two packages, wet_slimpattern provides a convenient approach. Using a plugin-based method, no modifications to Textpattern's core code are required – you simply upload this plugin through the usual plugin administration interface. Additionally, you can toggle statistics logging by simply enabling or disabling this plugin. No need to edit `index.php` anymore.

### Usage:

**wet\_slimpattern** assumes that you have previously installed SlimStat successfully. You can omit the final step of SlimStat’s installation which would direct you to include the hit logging code `inc.stats.php` somewhere into your pages.

Instead, install wet\_slimpattern and enable it. Logging should start immediately whenever your website attracts visitors. If you chose to install SlimStat into a different folder that the default `/slimstat/` you will need to edit this plugin in Textpattern’s plugin administration screen and change the line reading

`$statslogger = "/slimstat/inc.stats.php";`

to reflect the actual path you chose.

The list of ignored URLs and query strings is kept in a [regular expression](https://www.regular-expressions.info/) just at the head of the plugin code. By default, all feed URLs are exluded from logging. Expand to your liking…

`$ignore = '/\\/&|^\\/rss\\/|^\\/rss$|^\\/atom\\/|\[...\];`

### Licence

This plugin is released under the [Gnu General Public Licence](https://www.gnu.org/licenses/gpl.txt).

### Download

Get it here: [Code Is Pottery | Robert Wetzlmayr](https://wetzlmayr.at/awasteofwords/?c=code-is-pottery).

### Resources and Relateds

Express your suggestions, report bugs and discuss enhancements in this [thread](https://forum.textpattern.com/viewtopic.php?id=13553) in the Textpattern forum.

### Change log

| Date       | Version | Notes                                                                               |
|------------|---------|------------------------------------------------------------------------------------|
| 2005-12-26 | 0.1     | Initial release                                                                     |
| 2006-07-05 | 0.3     | Customizable filter for URLs and query strings                                     |
| 2007-03-01 | 0.4     | URL and query string filter employs [regular expressions](http://www.regular-expressions.info/) |
| 2007-03-02 | 0.4.1   | Fix brainless typo...                                                               |
