# Limitations

PDF is a very feature rich file format, and PdfToSvg.NET does not support all of them. If a PDF is using an unsupported feature, the output might not look identical to what you see in other PDF readers.

This is a incomplete summary of non-supported features.

## Image formats

The by far most commonly used image formats in PDFs are images encoded with DCTDecode (JPEG) and FlateDecode (PNG alike). Those are supported, with the exception that DCTDecode is only supported for RGB images.

The following image formats are not supported:

* CCITT Fax
* JPEG 2000
* CMYK JPEG
* JBIG2

## Color spaces

The commonly used color spaces are supported and transformed to RGB. PDF does however support a lot of color spaces, and not all of them are supported. If an unsupported color space is encountered, you might see areas that are black, but shouldn't be.

Non-supported color spaces:

* Pattern
* ICCBased

## Other features

The following features are not supported:

* Blending modes
* PDF forms
* Embedded JavaScript
* Annotations
* Document links
