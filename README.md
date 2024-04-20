# Infinite Scroll

The "Infinite Scroll" website is a dynamic platform that showcases images fetched from the Unsplash API, allowing users to scroll through an endless collection of images.

## Key features and technologies used in the development of the Quote Generator include:

### Infinite Scrolling:

Implemented to provide a seamless browsing experience, where new images are loaded as the user scrolls down, reaching 1000 pixels from the bottom of the page.
This technique enhances user engagement by continuously updating the content without requiring manual refreshes.
Code snippet:

```js
window.innerHeight + window.scrollY >= document.body.offsetHeight - 1000;
```

The expression checks if the sum of the viewport height and the scroll position is greater than or equal to the height of the `<body>` element minus 1000 pixels.
If this condition is true, it means the user has scrolled to a point where the bottom of the viewport is within 1000 pixels of the bottom of the page.

### Dynamic Quote Fetching:

Utilizes the await fetch method to retrieve quotes from the Unsplash API providing new images and new experiences on every website load and nearly every scroll.

### Performance Optimization:

Incorporates a mechanism to check if images are loaded and limits the number of images loaded at a time.
This approach is particularly beneficial for devices with slower internet connections, ensuring that users can view some images while waiting for the next batch to load, thereby improving the overall user experience.

### Responsive Design:

Employs CSS media queries to ensure the website is optimized for both tablets and mobile phones by reducing the font size and margins around the images for a better mobile user experience.
