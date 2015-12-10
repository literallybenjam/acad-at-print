#  acad@print

Formats a webpage like an academic essay when it is printed, through the use of `@page` and CSS Media Queries.

12pt times, double-spaced, page numbers in the top-right, 1in margins, all that fun stuff.

Doesn't affect screen display at all, but wipes anything in the following pseudo-elements when you print:

- html::before
- html::after
- body::before

Headers and footers require support for `columns`.

##  Usage:

Just include `style.css` in the webpage.

You can set metadata on the `<body>` element to add a header to your document:
- `data-acad-author`
- `data-acad-date`
– `data-acad-professor`
- `data-acad-course`

In addition, you can set metadata on the `<html>` element to modify the headers and footers:
- `data-acad-tl` : Top-left
- `data-acad-tm` : Top-middle
- `data-acad-tr` : Top-right
- `data-acad-bl` : Bottom-left
- `data-acad-bm` : Bottom-middle
- `data-acad-br` : Bottom-right
- `data-acad-pagepos` : Page number position. Must be one of : `none` `tl` `tm` `tr` `bl` `bm` `br`. Defaults to `none`.
- `data-acad-headalign` : Text-alignment for header. Must be one of `right` `center` `left`. Defaults to `center`.
- `data-acad-footalign` : Text-alignment for footer. Must be one of `right` `center` `left`. Defaults to `center`.

`<aside>s`, `<nav>s`, and any element with the attribute `data-acad-hidden` will not be displayed.
