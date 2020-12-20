# Homework01-Code-Refactor

Changed the title (was previously titled "website") and added a meta tag (with content description) in the head tag to increase accessibility and improve search engine results.

Changed the div tags to section tags throughout the html file for improved accessibility and readability. Made necessary adjustments to style.css file in order to maintain proper formatting and functionality.

Example: Changed everything in the section class="header" on the style.css file, from

a div tag to a section tag.

I added nav tags around the unordered list, in order to indicate that the unordered list acts as a set of navigational links.

The image in the "hero" class, was previously located on the style.css file as a background image. I moved it to the html file and added alt text for improved accessibility.

In addition, I added the ".hero img" styling to the style.css file, and "object-fit:contain", so that the image would fit within its parent container.

* At the time, this seemed like a better practice and made more sense than having an empty div section on the html page. Since the image is purely decorative, I am no longer sure if this step was necessary. In addition, this led to multiple formatting issues that had to be fixed in order for the image to display properly.

I added alt text to all images on the webpage for improved accessibility. For the images located in the section class="benefits" that were of little importance, I added null alt text (alt= " ") so that they would be ignored by assistive technologies.
6.The search-engine-optimization" link was broken, and was not redirecting to the corresponding section because it was only assigned a class, and not an ID. To correct the issue, I added the id= "search-engine-optimization", so that it would navigate properly.

Each image tag located within section class="benefits, had the same styling on the style.css file, but was listed separately. I added the class ".benefits img" to the style.css page in order to condense them and avoid redundancy.

For organizational purposes, I rearranged items on the CSS page in descending order, matching their order on the HTML page. I regrouped items belonging to the same parent class on the style.css file, giving it a more logical flow, and allowing anybody viewing the code to easily find items.

Example: Everything in the section class: "social-media-marketing", is now grouped together on the style.css file.

.social-media-marketing

.social-media-marketing h2

.social-media-marketing img

This was done for all classes located under the parent section class="content".

I added comments throughout the HTML and CSS files to make it easier for the next person to identify sections, classes, groupings etc.
