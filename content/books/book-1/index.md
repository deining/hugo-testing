+++
title = 'Book 1'
date = 2023-01-18T15:55:26-08:00
draft = false
+++

## Images

### Image from a page resource

`![Kitten A](a.jpg "This is Kitten A")`

![Kitten A](a.jpg "This is Kitten A")

### Image from a global resource

`![Kitten C](/images/c.jpg "This is Kitten C")`

![Kitten C](/images/c.jpg "This is Kitten C")

### Images from a remote resource

`![Kitten D](https://www.mooring.com/tests/images/d.jpg "This is Kitten D")`

![Kitten D](https://www.mooring.com/tests/images/d.jpg "This is Kitten D")

### Images with wrapping `p` tags removed and markdown attributes

```x
![Kitten A](a.jpg "This is Kitten A")
{.my-class #my-id style="border: 2px solid #333;"}
```

![Kitten A](a.jpg "This is Kitten A")
{.my-class #my-id style="border: 2px solid #333;"}

## Links

### Link to another page

`[Post 1](/posts/post-1 "Link to Post 1")`

[Post 1](/posts/post-1 "Link to Post 1")

### Link to a page resource

`[PDF B](b.pdf "Link to PDF B")`

[PDF B](b.pdf "Link to PDF B")

### Link to a global resource

`[PDF A](/docs/a.pdf "Link to PDF A")`

[PDF A](/docs/a.pdf "Link to PDF A")

### Link to a remote resource

`[Remote PDF](https://www.mooring.com/tests/media-types/samples/a.pdf "Link to remote PDF file")`

[Remote PDF](https://www.mooring.com/tests/media-types/samples/a.pdf "Link to remote PDF file")

## SVG images

### SVG image from a page resource

`![Ford Focus](d.svg "This is a Ford Focus")`

![Ford Focus](d.svg "This is a Ford Focus")

### SVG image from a global resource

`![Penrose staircase](images/e.svg "This is an impossible staircase")`

![Penrose staircase](images/e.svg "This is an impossible staircase")

### SVG image from a remote resource

![A car](https://www.mooring.com/tests/media-types/samples/svg.svg "This is a car")
