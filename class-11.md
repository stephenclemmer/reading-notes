# Audio, Video, Images

## Video and Audio Content

**Explain how the ability to use video and audio on the web has evolved since the early 2000s.**
Now depricated techniologies like FLash player have been replaced with the native solutions that came out with the advent of HTML5. 

**Describe the use of the src and controls attributes in the \<video> element.**
In the same way as for the \<img> element, the src (source) attribute contains a path to the video you want to embed. It works in exactly the same way.

**Why is it important to have fallback content inside the \<video> element?**
 Fallback content will be displayed if the browser accessing the page doesn't support the \<video> element, providing a fallback for older browsers. It's analagoung to the alt text that would be displayed if an image wasn't able to be linked to.

**Write a very short story where \<audio> and \<video> are characters.**

Once upon a time audio and video went on atrip. Audio told great stories. Video demonstrated all sorts of interesting things. They found that each took up a large amount of bandwidth, so they each went to their rooms and embedded for the night.

## A Complete Guide To Grid

**How does Grid layout differ from Flex?**
The basic difference is that flexbox works one dimensionally, while grid works two dimensionally. 

**Grid container, grid item, and grid line are a few important terms to understand when using Grid. Please describe these terms in a few sentences.**
Grid Container: This is the parent element upon which the grid is applied. This is similar to how flex must be applied to the parent element so that its children are affected.

Grid Item: These are the direct decendents of the grid container, which will be styled by using Grid. This is similar tpo how flex affects elements.

Grid Line: These are the dividing lines that make up the structure of the grid. They can run either vertically or horizontally.

## Responsive Images

**Besides making a site visually appealing across different screen sizes, why should developers make images responsive?**
Visually responsive images allow devices to choose the image that is the correct size and resolution, so the objects in the images which one wants the user to enjoy are framed appropriately. Also, using responsive images means that they will be loaded before the CSS and JS are done loading which will ensure that processing happens more efficiently.

**Define the following \<img> attributes srcset and sizes. Write an example of how they are used.**

srcset defines the set of images one allows the browser to choose between, and what size each image is. 

sizes defines a set of media conditions (e.g. screen widths) and indicates what image size would be best to choose, when certain media conditions are true

**How is srcset more helpful for responsive images than CSS or JavaScript?**
When the browser starts to load a page, it starts to download (preload) any images before the main parser has started to load and interpret the page's CSS and JavaScript. This means that CSS and JavaScript are too slow to serve up the appropriately sized image for the screen that it will be displayed on. srcset is able to provide the information needed for the correct image to be chosen so that everything displays properly from the outset. 
