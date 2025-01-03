# Uncommon HTML Bug: Incorrect use of textContent
This repository demonstrates a subtle bug related to accessing text content within HTML elements using JavaScript.

## Description
The bug involves the incorrect usage of `textContent` to retrieve the text content of an HTML element.  `textContent` returns the entire text content, including the text within any child elements.  If you only need the visible text without child tags, use `innerText` instead.

## Bug
The `bug.html` file contains the buggy code.  It attempts to retrieve the text content using `textContent` and prints it using an alert. However, this will show the text content including any tags.

## Solution
The `bugSolution.html` shows the corrected code. It uses `innerText` to get only the visible text, which is the intended behavior in most cases.