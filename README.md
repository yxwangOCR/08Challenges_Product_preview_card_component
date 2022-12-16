# Frontend Mentor - Product preview card component solution

This is a solution to the [Product preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/product-preview-card-component-GO7UmttRfa).

## The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover and focus states for interactive elements

## Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow

## Screenshot

![](design/active-states.jpg)
![](design/mobile-design.jpg)

## Useful tips + examples

[Picture Element](https://www.w3schools.com/html/html_images_picture.asp)

```html
<picture>
  <source media="(min-width: 992px)" srcset="desktop-image.jpg" />
  <source media="(min-width: 350px)" srcset="mobile-image.jpg" />
  <img src="mobile-image.jpg" />
</picture>
```

```css
picture img {
  /*Image Style Here*/
}
```

[Picture Srcset not working?](https://stackoverflow.com/questions/39236087/html5-picture-element-does-not-seem-to-be-supported-by-chrome-52-srcset-not-wor/71893074#71893074)

- <strong>Tip 1 </strong>: The img element inside the picture element isn't optional. The picture wrapper and its source elements are there to change the img, not replace it.

- <strong>Tip 2 </strong>: You must set a max-width for the lower width image, otherwise it is the only one always served (you can see it in devtools network tab if you try).

```html
<picture>
  <source media="(min-width: 992px)" srcset="large.jpg" />
  <source media="(max-width: 991px)" srcset="medium.jpg" />
  <img src="small.jpg" alt="" />
</picture>
```

[Text alternatives for images](https://www.w3.org/WAI/tutorials/images/)

- <strong>Tip 3 </strong>: Images must have text alternatives that describe the information or function represented by them. This ensures that images can be used by people with various disabilities.

```
Why is this important?
```

- People using screen readers: The text alternative can be read aloud or rendered as Braille
- People using speech input software: Users can put the focus onto a button or linked image with a single voice command
- People browsing speech-enabled websites: The text alternative can be read aloud
- Mobile web users: Images can be turned off, especially for data-roaming
- Search engine optimization: Images become indexable by search engines
