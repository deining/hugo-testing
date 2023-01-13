+++
title = 'Hugo GitHub Issue #10606 (de)'
date = 2023-01-13T10:18:10-08:00
draft = false
details = 'https://github.com/gohugoio/hugo/issues/10606'
description = "Clearly document how to compute URLs that are `baseURL` aware, both for theme and site designers"
+++

Characteristics of this site that affect URLs:

- Multilingual
- Served from a subdirectory
- Permalinks set in site configuration
- Slugs set in content front matter

All rendered URLs are obtained from the `.RelPermalink` method on pages and resources. That includes:

- Internal markdown links to pages and files (external links not touched)
- Internal and external markdown images (also sets `width` and `height` attributes)
- Menu entries (via `pageRef`)
- CSS files
- CSS properties (e.g., `background-image: url("/images/a.jpg")`)
- JavaScript files
- Favicon


None of the URLs are hard-coded, and none of them are passed through the `relURL` or `relLangURL` function.

See [Post 2](/posts/post-2) for examples of image processing based on the destination query string.

----
