# Responsive Images

## Knowledge Check

### What is the main difference between object-fit and background-size?

The main difference would be on where its used object-fit is for `<img>` elements while the background-size property is for images set as a background-image.

### How can you define a width and a height on an img without distorting it?

One way is not to define both of them at the same time, or you can use the `object-fit`, `background-size` and `background-position` property

### Why would you want to provide different images at different screen resolutions?

Because images can look different on different screen resolutions, it might look good on a desktop environment, but it can look ugly on mobile since it might be cropped or it's too big for a mobile resolution, by providing different images we can show the user a better image that will suit on their device.

### When would you want to use an img with a srcset vs a picture?

If you are only serving the same image with a different size, it's better to use an img with a srcset as it's more performant vs picture.