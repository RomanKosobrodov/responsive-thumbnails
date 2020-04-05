# Responsive Gallery Example

A small example of responsive image gallery desing using flex box, media queries and CSS variables.The images are taken from [Flickr](https://www.flickr.com/) and [Unsplash](https://unsplash.com/).

## Demo

See the example [live](http://responsive-thumbnails.kosobrodov.net).

## Implementaion

There are a few simple tricks in the code. To fit an image of unknown aspect ratio into a fixed box with ratio 2/3 use the following:

```css
img {
  max-width: var(--image-width);
  max-height: calc(var(--image-width) * 2 / 3);
  width: auto;
  height: auto;
}
```

Another technique that I find useful is the `calc` function combined with CSS variables as shown in the example code above.
