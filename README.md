# INFO-6123 - Web Design Project
### Kaleb Jubar - A-Plus Construction
This website consists of a landing and contact page for a home construction, estimation, and contracting company called A-Plus Construction.

The website was fully designed and coded by me, including wireframes and high-fidelity mockups made with Figma to guide the development process so that I didn't waste time writing, deleting and rewriting code I wasn't happy with. You can see the design documents in the `design/` folder.

The images used are stock images obtained from various sites on the internet, each of which are documented in the `sources.txt` files. If an image was edited (such as darkening the banner images or cropping the service images), this was also documented in `sources.txt`. The burger menu icons were created by me, and the website logo was designed and created by my brother, Tyler.

The mobile version of the website features a collapsible navigation menu that was implemented entirely via HTML/CSS. I spent some time trying to figure out how to animate it, but it wasn't possible to get something completely smooth without using JavaScript, so the menu is currently not animated. Either way, I thought this was a neat additional feature to add to the website.

The code features detailed comments where necessary, as well as category divisions for the CSS to keep everything organized. This should hopefully explain any technical decisions or novel solutions I came up with for this project. There are a few snippets of code that were adapted from StackOverflow solutions, if I was unable to figure them out on my own; these references are documented in the comments related to the code snippet. If you have any questions about my implementation of the website, feel free to email me at k_jubar@fanshaweonline.ca and I would be happy to explain.

## Design Principles
### Contrast and Color Scheme
I decided on a color scheme consisting of shades of teal and orange, as these felt appropriate for a construction company. This includes light and dark variants of both to allow proper contrast, and also includes white and light gray for layout elements.

### Proximity
Both the mobile and desktop variants of the website were designed with a consistent flow in mind, with enough whitespace to keep it from looking cluttered, but not too much to the point that it's empty. The page is broken up into specific sections with banner images and headings to improve readability, as well.

### Typography
The fonts used were carefully chosen to convey the proper feeling of the website - professional, but approachable. I chose a serifed display font for the headings to give it a somewhat formal look, with a plain (and specifically not cartoony or whimsical) sans-serif font for the rest of the page. The logo uses a special display font that I felt gave it a good construction vibe. On the mobile version of the website, the font size of smaller text elements (like `<p>`, `<a>`, etc.) is increased to improve readability.

## Accessibility
This website meets accessibility standards in a few different ways. For starters, it meets basic recommendations for accessibility of a webpage. It includes a `lang` attribute on the `html` tag, `alt` text for any images, and has proper closing tags and structure for all HTML tags. In addition, any elements that have a background image set via CSS use the `title` attribute to define alternate text for screen readers.

The color scheme of the website naturally lends itself to being more appropriate for colorblind users, specifically those with protanopia and deuteranopia. Colorblind filters for these two types of colorblindness are typically blue/teal and orange; this means that all elements used in the page (other than the images) should be easily readable for colorblind users.

In addition to the above accessibility considerations, I also used the WebAIM WAVE accessibility evaluation tool to resolve accessibility errors in the website. An example of one such change is adding a `<label>` element to the header that is associated with the burger menu to give context to screen readers (the element is only shown to screen readers via `aria-hidden="false"` attribute, not sighted users, as it would be redundant).

## Search Engine Optimization
At a base level, the headers and content of the webpages use keywords important for identifying the webpage as a construction and contracting site. This includes proof terms for the contracting industry as well as some long-tail buzzwords. In addition to this, I added `<meta>` tags with keywords and a description to the `<head>` of both pages.