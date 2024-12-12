+++
{{- /* Archetype for a blog post with an image */}}
{{- /* Usage: `$ hugo new content blog/2023-01-31_post-name.md` */}}
{{- /* Note: Make sure to: */}}
{{- /*   - place an underscore between the date and the slug */}}
{{- /*   - add an .md suffix */}}
{{- $filename_parts := split .File.ContentBaseName "_" }}
title = '{{ replace (index $filename_parts 1) "-" " " | title }}'
date = '{{ index $filename_parts 0 }}'
slug = '{{ index $filename_parts 1 }}'
draft = true
author = "Erik Hansen"
+++

## Heading One

This is the first paragraph.

_This_ is a list:

- first
- second
- third

This is some `code`:

```js
console.log(`Today is ${Date.now()}`)
```
