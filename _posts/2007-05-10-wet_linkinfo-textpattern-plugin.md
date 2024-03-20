---
layout: post
title: "wet_linkinfo: Textpattern plugin to extract a managed link's properties"
---
**wet_linkinfo** is a plugin for [Textpattern](https://textpattern.com/) which takes a link id number and returns either the results of parsing a form passed by attribute, parsing the contained text, or one of these assigned properties:

- date
- category
- url 
- linkname
- linksort
- description

### Usage

`<txp:wet_linkinfo id="2" />` 

- or -

`<txp:wet_linkinfo id="2">...other contained tags and text...</txp:wet_linkinfo>`

### Required attributes

| attribute | description | default |
|-----------|-------------|---------|
| **id** | The link's numerical `id` as listed in the links page. | None. |

### Optional attributes

| attribute | description | default |
|-----------|-------------|---------|
| **type** | Either "date", "category", "url", "linkname", "linksort", or "description". | `"url"` |
| **escape** | Replace special characters with their HTML entities. | Empty. |
| **form** | A form's name which will be parsed to produce the tag's output. The form can contain any text, HTML elements, or Textpattern tags, and will produce reasonable results when one of these tags is encountered: <ul><li>[txp:link](https://docs.textpattern.com/tags/link)</li><li>[txp:link_category](https://docs.textpattern.com/tags/link_category)</li><li>[txp:link_date](https://docs.textpattern.com/tags/link_date)</li><li>[txp:linkdesctitle](https://docs.textpattern.com/tags/linkdesctitle)</li><li>[txp:link_name](https://docs.textpattern.com/tags/link_name)</li><li>[txp:link_url](https://docs.textpattern.com/tags/link_url)</li><li>[txp:link_description](https://docs.textpattern.com/tags/link_description)</li></ul> | Empty. |

### Sample use

| tag | function |
|-----|----------|
| `<txp:wet_linkinfo id="3" type="url" />` | Return a link's URL |
| `<txp:wet_linkinfo id="3" type="description" escape="html" />` | Return a link's description and replace special characters with HTML entities. |
| `<txp:wet_linkinfo id="3" form="mylinkinfo" />` | Return the result of parsing the form named "mylinkinfo". Create a form of type `link` and put something useful in it. |
| `<txp:wet_linkinfo id="3"><txp:link /><br /><txp:link_date /></txp:wet_linkinfo>` | Return a link and its creation date, separated by a line break. |

### Licence

This plug-in is released under the [Gnu General Public Licence](http://www.gnu.org/licenses/gpl.txt).

### Download 

Get it here: [Code Is Pottery − Robert Wetzlmayr](https://wetzlmayr.at/awasteofwords/?c=code-is-pottery).

### Resources and Relateds

Express your suggestions, report bugs and discuss enhancements in this [Textpattern forum thread](https://forum.textpattern.com/viewtopic.php?id=22507).

### Change log

| Date | Version | Notes |
|------|---------|-------|
| 2007-05-10 | 0.1 | Initial release |
| 2007-05-25 | 0.2 | Add `form` attribute and container ability |
