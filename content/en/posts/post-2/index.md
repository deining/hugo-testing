+++
title = 'Post 2 (en)'
date = 2023-01-13T11:56:30-08:00
draft = false
slug = 'second-post-in-english'
+++

With optional parsing of the image destination query string, you can:

- Process the image using any of the image processing [methods] or [options]
- Include additional image element attributes (e.g., `class`, `id`, `loading`)

[methods]: https://gohugo.io/content-management/image-processing/#image-processing-methods
[options]: https://gohugo.io/content-management/image-processing/#image-processing-options

## Query string parameters

Key|Description|Type|Example
:--|:--|:--|:--
`a`|anchor|processing option|`smart`
`c`|class|element attribute|`my-class`
`f`|format|processing option|`webp`
`h`|height|processing option|`400`
`i`|id|element attribute|`my-id`
`l`|loading|element attribute|`lazy`
`m`|method|processing method|`resize`
`p`|preset|processing option|`photo`
`q`|quality|processing option|`75`
`r`|rotation|processing option|`180`
`w`|width|processing option|`600`
`bc`|background color|processing option|`ffaa33 or fa3`
`rs`|resampling filter|processing option|`lanczos`

Notes:

- Keys are case-sensitive
- Values are case-insensitive
- The default processing method is `resize`
- To add multiple classes, provide multiple `c` key/value pairs in the query string
- As with all query strings, the order of the key/value pairs is irrelevant
- The anchor, format, method, preset, quality, rotation, background color, and resampling filter are ignored with SVG images

## Examples

`![Kitten B](images/b.jpg?w=200&c=foo&c=bar)`

![Kitten B](images/b.jpg?w=200&c=foo&c=bar)

`![Kitten B](images/b.jpg?w=100&h=100&m=fill&rs=CatmullRom)`

![Kitten B](images/b.jpg?w=100&h=100&m=fill&rs=CatmullRom)

`![Kitten B](images/b.jpg?r=90&w=175)`

![Kitten B](images/b.jpg?r=90&w=175)

`![Kitten D](https://www.mooring.com/tests/images/d.jpg?w=250 "This is Kitten D")`

![Kitten D](https://www.mooring.com/tests/images/d.jpg?w=250 "This is Kitten D")

`![Ford Focus automobile](images/d.svg?w=200 "This is a Ford Focus")`

![Ford Focus automobile](images/d.svg?w=200 "This is a Ford Focus")

`![Penrose staircase](images/e.svg?w=250 "This is a Penrose staircase")`

![Penrose staircase](images/e.svg?w=250 "This is a Penrose staircase")

`![Jaguar automobile](https://www.mooring.com/tests/media-types/samples/svg.svg?w=300 "This is a Jaguar")`

![Jaguar automobile](https://www.mooring.com/tests/media-types/samples/svg.svg?w=300 "This is a Jaguar")
