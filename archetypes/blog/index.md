+++
{{- /* Archetype for a blog post with an image */}}
{{- /* Usage: `$ hugo new content blog/2023-10-27_post-name` */}}
{{- /* Note: Make sure to: */}}
{{- /*   - place an underscore between the date and the slug */}}
{{- /*   - leave off the .md suffix */}}
{{- $filename_parts := split .File.ContentBaseName "_" }}
title = '{{ replace (index $filename_parts 1) "-" " " | title }}'
date = '{{ index $filename_parts 0 }}'
slug = '{{ index $filename_parts 1 }}'
draft = true
author = "Erik Hansen"
+++

## New blog post from a page bundle

This is the first paragraph.

{{< figure src="picture.jpg" alt="Description of this picture" title="The caption for this picture" >}}
