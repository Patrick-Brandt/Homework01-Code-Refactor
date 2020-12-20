# Homework01-Code-Refactor

This is my first homework assignment for the University of Washington Coding Bootcamp. The assignment was to take existing code for a webpage (we were given an HTML file and a CSS file to work with), and refactor it so that the webpage meets accessibility standards. 

# Here was the acceptance criteria provided:

- Given a webpage meets accessibility standards
- When I view the source code, then I find semantic HTML element.
- When I view the structure of the HTML elements, then I find that the elements follow a logical structure independent of styling and positioning.
- When I view the image elements, then I find accessible alt attributes.
- When I view the heading attributes, then they fall in sequential order.
- When I view the title element, then I find a concise, descriptive title.

# Here are the following changes that I made to the code provided:
 
1. Changed `<title>` (was previously titled “website”) and added a `<meta>` tag (with content description) in the `<head>` to increase accessibility and improve search engine results.
 
2. Changed the `<div>` tags to `<section>` tags throughout the html file for improved accessibility and readability. Made necessary adjustments to style.css file in order to maintain proper formatting and functionality. 

Example- I changed everything in the `<section class="header">` on the style.css file, from `<div>` to `<section>`.
  
3. I added `<nav>` tags around the `<ul>`, in order to indicate that the unordered list acts as a set of navigational links. 

4. The image in the “hero” class, was previously located on the style.css file as a background image. I moved it to the html file and added alt text for improved accessibility. In addition, I added the “.hero img” styling to the style.css file, and “object-fit:contain”, so that the image would fit within its parent container.
	
	 -At the time, this seemed like a better practice and made more sense than having an empty `<div>` section on the html page. Since the image is purely decorative, I am no longer sure if this step was necessary. In addition, this led to multiple formatting issues that had to be fixed in order for the image to display properly.

5. I added alt text to all images on the webpage for improved accessibility. For the images located in the `<section class=“benefits”>` that were of little importance, I added null alt text (alt= “ “) so that they would be ignored by assistive technologies.

6. The `<a href="#search-engine-optimization”>` link was broken, and was not redirecting to the corresponding `<section>` because it was only assigned a class, and not an ID. To correct the issue, I added `<id=“search-engine-optimization”>`, so that it would navigate properly.

7. Each `<img>` tag located within `<section class=“benefits>`, had the same styling on the style.css file, but was listed separately. I added the class “.benefits img” to the style.css page in order to condense them and avoid redundancy.

8. For organizational purposes, I rearranged items on the CSS page in descending order, matching their order on the HTML page. I regrouped items belonging to the same parent class on the style.css file, giving it a more logical flow, and allowing anybody viewing the code to easily find items. 

  Example- Everything in `<section class="social-media-marketing">` is now grouped together on the style.css file.
  ```
  .social-media-marketing
  .social-media-marketing h2
  .social-media-marketing img		
  ```
  This was done for all classes located under the parent `<section class=“content”>`.

9. I added comments throughout the HTML and CSS files to make it easier for the next person to identify sections, classes, groupings etc.

#
