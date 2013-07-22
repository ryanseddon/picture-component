# Picture component

An implementation of the proposed `<picture>` element. See [original repo](https://github.com/scottjehl/picturefill) for something to actually use in production.

## How to use

This web component uses the Polymer library.

1. Make sure you have Polymers `platform.min.js` included in your page
1. Import component `<link rel="import" href="x-picture.html" />`
1. A picture element is contained inside a `<x-picture>` element
1. For each sized image specify as `<x-source>` inside `<x-picture>`

```html
<x-picture alt="A giant stone face at The Bayon temple in Angkor Thom, Cambodia">
    <x-source src="imgs/small.jpg"  media="(min-width: 200px)"></x-source>
    <x-source src="imgs/medium.jpg" media="(min-width: 400px)"></x-source>
    <x-source src="imgs/large.jpg"  media="(min-width: 800px)"></x-source>
</x-picture>
```

## Experiment only

Please don't use this, that's what the [picturefill](https://github.com/scottjehl/picturefill) polyfill is for. This version is missing default image support and image swapping on resize.

## Made as part of talk

I did a talk on Web Components and created a whole bunch of components to dog food the talk itself. See master repo [web-components](https://github.com/ryanseddon/web-components).
