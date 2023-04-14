---
layout: post
title: Textpattern, a Slim Content Management System (CMS) Between TYPO3 and WordPress
---

## The Middle Ground Between TYPO3 and WordPress

How to choose from the unmanageable abundance of content management systems the one that fits the task, can be mastered with a manageable learning effort and will not become too narrow, too small or too sluggish in the future? No easy task. Often one orients oneself to well-known names or to the frequency of specialist book publications on a CMS. From the open source camp, one therefore chooses either [Joomla!](https://www.joomla.org/) or [Typo3](https://typo3.org/) for the corporate site of MultiMega AG, or [WordPress](https://wordpress.org/) for the small personal blog.

But what about something in between?

[Textpattern](https://textpattern.com/) is a free, lightweight CMS that can be installed within ten minutes on the usual web hosting plan with Apache, PHP and MySQL. 

Its optimal field of application is blogs and websites for small and medium-sized enterprises or freelancers. As open source software, Textpattern is subject to the GPL and is therefore freely available and free to use.

## Publish texts easily on the Internet

The name says it all: Textpattern is a tool for authors whose focus is on text. The indications are clear: the central element is "articles", which essentially consist of an excerpt, the actual article text and some administrative properties for categorising and dating. Once you have successfully logged in to Textpattern's administration interface, you land directly in the form for entering a new article and can start writing straight away.

## Administration of a website with Textpattern

Content is entered either in ordinary XHTML or - more simply - in the markup language "Textile". Textile has an easy-to-learn syntax for marking up headings, lists or quotations and automates the technical niceties such as the correct closing of tags. The well-known WYSIWYG editor TinyMCE can be retrofitted via an extension.

## The building blocks of the content management system

To arrive at a displayable XHTML page, Textpattern uses various content building blocks stored in its database:

* Articles with their associated comments
* Images with their associated thumbnails
* Links
* Downloadable files

Up to two user-defined categories can be assigned to each of these elements. The database also contains other more "administrative" components:

*   Page templates
*   Style sheets (CSS)
*   Code for extensions and plugins
*   User management with rights assignment
*   Reusable code or layout blocks
*   Access log

The aforementioned content blocks are filtered from the database using Textpattern tags. For example, the `<txp:article />` tag filters all articles assigned to a specific section. Tags can be combined in forms and mixed with CSS. Some are placed directly in the page template.

An interactive tag builder helps beginners explore the possibilities. The Textbook wiki provides a list of all tags and their attributes, as well as a fairly comprehensive collection of instructions for installing and administering a Textpattern-based website, considering its open-source nature.

## Web Design According to World Wide Web Consortium Standards

Of course, Textpattern supports web design according to accepted standards, allowing for layouts without HTML tables and separating content from styling. It also supports the use of accepted technologies such as RSS and backend compatibility with all popular browsers.

In terms of site structure and URL design, Textpattern supports dynamic switching between multiple methods, including the "user-friendly" variants popular with users and search engines:

*   `http://example.com/year/month/day/article-title`
*   `http://example.com/section/article-title`

If the web server technology does not support URL rewrites, "messy" URLs are used:

*   `http://example.com/index.php?id=42`

In accordance with the principle of "little work for the author", these URLs are automatically derived from the titles of the articles. Umlauts or other invalid characters are smoothed out. If visitors remain disoriented despite this catchy structure and good accessibility for search engines, the integrated full-text search helps.

## Individual solutions for web sites

Textpattern has a very structured administration interface. Plugins for Textpattern can be easily installed and even the backend can be extended. Besides the already mentioned possibility of using a WYSIWYG editor instead of the standard text filter, plug-ins for caching for high-traffic sites, for integrating the popular "Web 2.0" icons like YouTube, digg.com or del.icio.us or for managing mailing lists shine. The plug-in spectrum is extremely wide. A comprehensive directory with detailed information and download addresses can be found on the Textpattern Resources site.

## A "wooly lizard" that nevertheless does not lay any eggs

Although Textpattern can in principle be extended almost arbitrarily with plug-ins, there are requirements that tend to push the system against the grain. For example, Textpattern lacks viable concepts for multilingual websites or sophisticated workflow features of larger systems such as version management or internal to-do lists for authors. A finely granulated permission rights system is not available and cannot be retrofitted. The Textpattern community is still waiting for a simple connection to shop solutions that go beyond a simple shopping cart.

"Dress for the moment" - i.e. the spontaneous, end-user-friendly change of site styling that make WordPress so attractive via themes - is in the vague planning phase. The ready-made templates downloadable from Textgarden.com must therefore be installed by the site designer with some manual intervention.

## Conclusion

Textpattern is a lean, flexible blog CMS that can be used to create very individual websites. The learning curve is not steep compared to many large CMSs.
