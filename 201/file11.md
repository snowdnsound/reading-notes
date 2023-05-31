# Audio, Video, Images

The <"video"> element allows you to embed a video very easily. 

In the same way as for the <"img"> element, the src (source) attribute contains a path to the video you want to embed. It works in exactly the same way.

The paragraph inside the <"video"> tag is called fallback content. This will be displayed if the browser accessing the page doesn't support the <"video"> element, allowing us to provide a fallback for older browsers. This can be anything you like; in this case, we've provided a direct link to the video file, so the user can at least access it some way regardless of what browser they are using.

## Things I Want to Learn More About

* Responsive design
* Live stream implementation 
* Video controls

## Handy Links

* [Audio and Video Content](https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Video_and_audio_content)
* [A Complete Guide to Grid](https://css-tricks.com/snippets/css/complete-guide-grid/)
* [Resonsive Images](https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Responsive_images)
* [Images in HTML](https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Images_in_HTML)
* [Responsive Design](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Responsive_Design)
* [Flexbox vs Grid](https://css-tricks.com/quick-whats-the-difference-between-flexbox-and-grid/)

## Questions From the Reading

### Video and Audio Content

Explain how the ability to use video and audio on the web has evolved since the early 2000s?

* We now are able to stream media live to the web, perform real-time communication and use HD/UHD quality video.

Describe the use of the src and controls attributes in the <"video"> element?

* It works like the img element, and contains the path to the video. Controls allow a user to control playback of the video. 

Why is it important to have fallback content inside the <"video"> element?

* So that the browser displays something, maybe a direct link, in case the browser is not able to play back the video.

Write a very short story where <"audio"> and <"video"> are characters?

* One character named audio is a sandwich ingredient. It like to be in sandiches with video, another ingredient. They taste really well together and audio effects the eaters ears, and video the eaters eyes as they take a bite. They can be combined to make endless sandwiches. 


### A Complete Guide To Grid

How does Grid layout differ from Flex?

* Flex is one-directional flow and has differnt use cases. Grid was created specifically for layouts. 

Grid container, grid item, and grid line are a few important terms to understand when using Grid. Please describe these terms in a few sentences?

* Grid container is the box that you work inside of. Grid item are the compents inside of the container that you affect. Grid line defines the width between your colums and rows. 

### Responsive Images

Besides making a site visually appealing across different screen sizes, why should developers make images responsive?

* It helps solve the art direction problem and resolution switching, so that useres have a smooth experience when browsing. 

Define the following <"img"> attributes srcset and sizes. Write an example of how they are used?

* Srcset defines the set of images that will be used, and their sizes. Sizes defines the media conditions So you might have a low and high res version of an image in your srcset attribute, and then sizes will tell the browser when to use which depending on your screen's size.

How is srcset more helpful for responsive images than CSS or JavaScript?

* It allows you to properly load images instead of how traditionall CSS and JavaScript load images. 
