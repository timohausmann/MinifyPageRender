# MinifyPageRender
Simple HTML minifier for ProcessWire.

This module hooks after Page::render and runs a simple minification. 

I mostly put this together for cosmetics. I like my `View source` neat and tidy.

This is not well tested yet, please open an issue if you run into problems.

## Minification code

The minify function source code was taken from StackOverflow:
https://stackoverflow.com/a/29363569/860205

Quote from the author: 

> This code removes redundant empty spaces. 
> Also it plays it safe and does not remove anything that could potentially break HTML, JS or CSS.

## Screenshot

![Alt text](/screenshot.png?raw=true "Screenshot of removed whitespace")

## Changelog

### 1.0.1

* Disabled one rule falsely removing whitespace in the character sequence `), something` like `(CEO), 2015`

### 1.0.0

* Initial release