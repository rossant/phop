# phop

A command-line photo manager in Python.

## Features

* Filter and sort photos
* Fast viewer (windowed and fullscreen)
* Set rating in XMP metadata

## Examples

```
phop view [files]  # view all photos
phop rating [files]  # print the rating
```

## Filtering and sorting

```
--sort name|date|star
--filter star>=3
--desc
--asc
```

## Keyboard shortcuts in view mode

* left/right to navigate
* F to toggle fullscreen mode
* S to star (rating=1)
* 1-5 to star
* escape to quit

## Random notes

How to get/set XMP rating in JPEG metadata with exiv2:

```
exiv2 "-Mset Xmp.xmp.Rating 1" test.jpg
exiv2 pr .\test.jpg -P X
```
