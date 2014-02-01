ymagik
======

A simple directive to let user add a picture by click or Drag and drop into an <image>

Usage
=====

* On desktop, click on image to display a file selector windows
* On mobile device, touch on it to display gallery or camera to take a picture directly
* Drag and drop image from desktop

How it works
============

An example is available on "example" directory

```html
<!-- Include Ymagik-->
<script src="ymagik.js"></script>
<!-- ... -->
<body>
<!-- ... -->
<div ymagik content-type="image.contentType" picture-content="image.base64" image-width="defaultWidth" default-image="defaultImageLink"></div>
<!-- ... -->
```

Parameters :
* picture-content : base64 value of the picture
* image-width : size of the image (on load, image will be resize to this width to avoid memory overload)
* content-type : on image load, this value is set with the detected value.
* default-image (optional) : link to the default image (use when picture-content && content-type are not set)

