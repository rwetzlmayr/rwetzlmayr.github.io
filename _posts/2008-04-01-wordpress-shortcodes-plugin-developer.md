---
published: true
title: WordPress shortcodes from the plugin programmer's point of view
layout: post
---
One of the innovations in WordPress 2.5 that remains rather inconspicuous compared to the equally acclaimed and spontaneously rejected administration interface is the Shortcode API. With this, WordPress has introduced a procedure, familiar from other CMSs, that allows authors to access complex functions directly from the body of a post using a simple "shortcode". To do this, simply enter the desired function in the text, enclosed in square brackets.

The first and only shortcode so far is `[gallery]`, which calls the new gallery function. In general, shortcodes are identified by square brackets containing a unique function identifier. Additional information is included in the shortcode via additional options: `[gallery size="medium" columns="4"]`. The options that shortcodes "understand" are determined by the creator of the function during programming. Shortcodes can be either self-closing (`[foo bar="baz"]`) or enclosing (`[foo bar="baz"]lorem ipsum[/foo]`).

Anyone who has worked with [Textpattern CMS](https://textpattern.com/) will immediately recognise the way the Textpattern tags work. No wonder, as the design and programming of the [shortcode API](https://web.archive.org/web/20080413105844/https://thresholdstate.com/threshold/4332/the-shortcode-api "The Shortcode API") was largely done by [Alex Shiels](https://flightpath.blog/), a former Textpattern developer.

Alex has abandoned the XML-based syntax of the Textpattern tags `<txp:foo bar="baz" />`. The author must therefore avoid collisions between terms in square brackets simply placed in the middle of the text and a shortcode with the same wording, for example, if he wants to write about the shortcode `[gallery]` and not include a gallery in the article.

I asked Alex about possible workarounds, and was advised to use the numeric HTML entities instead of the square brackets for "normal" text:

> Escaping shortcodes: good question. &#91;gallery&#93; works. We need a better way. - Alex Shiels

Attention: The numeric entities can only be entered in the HTML editor and will not survive a switch from the HTML editor to the visual editor.

So it looks like WordPress 2.5.1 (or whatever the next maintenance release is called) will bring an [escaping mechanism for shortcodes](https://trac.wordpress.org/ticket/6518). In the future, template designers should also be able to enjoy shortcodes - after all, working with PHP is not everyone's cup of tea...

