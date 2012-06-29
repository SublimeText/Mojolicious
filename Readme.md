# Description

This plugin has a syntax, completions, and snippets for working with Mojolicious (http://mojolicio.us) Embedded Perl templates.

# Completions

Inside a Embedded Perl block the following completions are available:

`<%`
`<%=`
`<%==`
`app`
`content`
`content_for`
`dumper`
`extends`
`include`
`flash`
`layout`
`layout`
`memorize`
`param`
`session`
`stash`
`url_for`
`title`
`base_tag`
`check_box`
`file_field`
`form_for`
`hidden_field`
`input_tag`
`javascript`
`link_to`
`password_field`
`radio_button`
`select_field`
`stylesheet`
`submit_button`
`tag`
`text_area`
`text_field`

# Perl Snippets

From a Mojolicious controller you can use these snippets:

`debug` -> `$self->app->log->debug(${1:'debug message'});`

`error` -> `$self->app->log->error(${1:'error message'});`

`mdump` -> `$self->app->log->debug($self->dumper(${1:object}));`


# Todo

* Default everything not in a Mojolicious block to HTML
* Add (more) stuff for Mojo::Lite
* Add Mojolicious helpers for inside Perl source
* Make awesomer

# Changelog

## June 28, 2012

* Resolved Issue #3 (and Issue #2). Adjusting syntax to use `source.js` and `source.css` syntax inside javascript/stylesheet blocks.
* Set a scope name (*entity.name.function.mojo*) on `begin` and `end` within EP tags

## June 25, 2012

* Resolved Issue #1. Added `JSON-tmLanguage` and `tmLanguage` syntaxes for Mojolicious' Embedded Perl in Perl `__DATA__` sections.
