# Salted [![License](https://img.shields.io/badge/license-MIT-blue.svg)](http://opensource.org/licenses/MIT)

## A responsive email template

Creating HTML email that renders well across most clients is surprisingly hard, especially when you want it to be responsive. Salted is a responsive email template that tries to make things easier.

Based on code originally developed by [Kevin Mandeville](http://twitter.com/KEVINgotbounce) and used in the [Litmus](http://litmus.com) email newsletters, Salted provides a base on which to build responsive HTML emails.

*Disclosure: I’m lucky enough to work for Litmus, one of the smartest groups of people around. Our emails typically take an opinionated approach to design and code, and the Salted template reflects that. Adapt as necessary!*

A lot of web designers are surprised by some of the stuff going on in HTML email, so here’s a breakdown of what you’ll find in the Salted template.

### Stacked Tables

At [Litmus](http://litmus.com), we love modularity. Being able to easily swap out pieces of our emails and work on sections in isolation is very important. Therefore, we tend not to nest tables too deep. Each horizontal section of the Salted template is its own table. You will find modules for a main hero section,  a single-column copy section, a two column grid section, and an article listing section, as well as both a header and footer.

Feel free to swap them out and adjust for your own purposes.

### Robust Images

Unfortunately, a lot of email clients block images by default. The images in the stacked tables are examples of how to properly code images for email—they include specific dimensions, ALT text, and styles for keeping your ALT text looking nice when images are disabled.

*Note: The images in the Salted template use relative paths, which will not work in real campaigns. Update your image paths to be absolute and point to a publicly accessible server to ensure that your subscribers get to look at all of your pretty graphics.*

### Bulletproof Buttons

Using images for buttons is so last season. To ensure that your calls-to-action display even when images are disabled, we use our own breed of bulletproof buttons throughout.

The buttons rely on thick borders for their structure, and some CSS3 for round corners. Using borders instead of padding on the table cell (our old approach) keeps the entire button tappable, not just the text inside. You can easily style the buttons using the inline styles, and adjust on mobile by targeting the *mobile-button* class.

### Responsive Goodness

The Salted template is fully responsive (so much as an HTML email can be). It uses fluid tables, fluid images, and media queries to adjust content and layout on mobile devices that support it.

*Be warned: If you thought the browser wars were bad, just wait until you start dealing with email clients. There are dozens of popular email clients that all support HTML and CSS to varying degrees. While the Salted template is very robust, it won’t look perfect in every client. That’s just the nature of the game.*

The *head* section of the email has a style block with all that good stuff going on. There are some client-specific resets (re: hacks) in there, as well as a general media query targeting screens below 525px. As always, test out your content and allow that to determine your breakpoints. This is just what works for us at [Litmus](http://litmus.com).

### Test Everything

While this code has been tested thoroughly through countless Litmus newsletter sends, when adapting it for your own purposes, I recommend you test the hell out of your campaigns. As mentioned before, email clients are a finicky bunch and you’re likely to run into issues at some point.

Naturally, I suggest sending your campaigns through [Litmus](http://litmus.com) for testing on dozens of different clients. It’s always a good idea to test on as many real devices as possible, too.

Enjoy!
