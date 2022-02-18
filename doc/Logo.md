<style>
img {
  height:150px;
  padding:1rem;
}
img[src*="#dark"] {
  background-color: gray;
}
img[src*="#mobile"] {
  border:1px dotted gray;
  height: 60px;
  padding: .5rem;
  width: 43px;
  object-position: 0 100%;
  object-fit: cover;
}
</style>

# All About the Logo <!-- omit in toc -->

![Minified Logo](/assets/logo-min.svg "Minified Logo 5kB")

![Logo Dark](/assets/logo-dark.svg#dark "Logo Dark Mode")

```css
.lgrad_blue,
.fill_green {
  fill: antiquewhite;
}
```

![Logo Mobile](/assets/logo-mobile.svg#mobile "Logo Mobile Mode")

```css
#phrase {
  display: none;
}
```

```xml
<svg xmlns="http://www.w3.org/2000/svg" width="600px" height="200px" >
  <defs>
   <linearGradient id="lgrad" x1="100%" y1="50%" x2="0%" y2="50%" >
          <stop offset="0%" style="stop-color:rgb(4,116,165);stop-opacity:1.00" />
          <stop offset="100%" style="stop-color:rgb(27,67,154);stop-opacity:1.00" />
    </linearGradient>
  </defs>
  <rect x="0" y="0" width="100%" height="100%" fill="url(#lgrad)"/>
</svg>
```

## References

1. [Online Gradient Generator](https://angrytools.com/gradient/)
2. [SVG Crop](https://svgcrop.com) Removes blank space from around SVG images.
3. [SVG Optimizer](https://svgoptimizer.com) It's all in the name.
