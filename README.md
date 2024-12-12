# Inconsistent Media Query Behavior with calc() function

This repository demonstrates an uncommon CSS bug related to using the `calc()` function directly within a media query's width condition.  The issue might lead to inconsistent behavior or lack of support in some browsers.

## Bug Description
The use of `calc(100vw - 100px)` in a `max-width` media query doesn't always work as expected across all browsers. While `calc()` is usually supported, its use with viewport units in media query conditions can be problematic.

## Solution
The recommended solution is to use JavaScript to calculate the viewport width and set a CSS custom property (or variable) that can be used in the media query.