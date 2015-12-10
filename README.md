#  acad@print

Formats a webpage like an academic essay when it is printed, through the use of `@page` and CSS Media Queries.

12pt times, double-spaced, 1in margins, all that fun stuff.
You'll have to do headers and footers through your browser settings until browsers start to support CSS definitions there.

Doesn't affect screen display at all, but wipes anything in the following pseudo-elements when you print:

- body::before

Headers and footers require support for `columns`.

##  Usage:

Just include `style.css` in the webpage.

You can set metadata on the `<body>` element to add a header to your document:
- `data-acad-author`
- `data-acad-date`
– `data-acad-professor`
- `data-acad-course`

`<aside>s`, `<nav>s`, and any element with the attribute `data-acad-hidden` will not be displayed.
