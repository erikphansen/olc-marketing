# Our Little Community marketing site

This project is the source for the [Our Little Community marketing site](https://ourlittlecommunity.org). It is built with [Hugo](https://gohugo.io).

## Running it locally

Run `hugo server -D`.

> The `-D` flag publishes drafts.

## Add a new blog post

Run `hugo new content blog/2023-10-27_post-name` to add a new blog post with a picture. This will create a new `2023-10-27_post-name` directory in the `content/blog` directory. Its starting content comes from the `archetypes/blog/` directory.

Alternatively, you could create a new blog post _without_ a picture by running `hugo new content blog/2023-10-27_post-name.md`. **Note:** This command includes a `.md` suffix, which the command mentioned before does not.

It's best practice to always use the first command, without the `.md` suffix, to create a new blog post in its own directory. Even if the blog post does not need images or other supporting files, giving each blog post its own directory will make it easier to add images later.

## Deploying

This project uses Github Actions to build and publish to Github Pages. So updating the [live site](https://ourlittlecommunity.org) is as simple as pushing to `master`.
