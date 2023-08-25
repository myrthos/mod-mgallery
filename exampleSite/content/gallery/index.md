---
title: Gallery
description: Example for gallery
date: 2023-05-20
---
<!-- Cspell:ignore ovlpos ovlx ovly ovlperc lightbox mgallery Hinode shortcode -->

To show this gallery properly in this example site, additional bootstrap classes are needed to wrap the gallery in.
For this purpose the mgallery shortcode is called with `hinode="false"`.

## Grid layout

{{< mgallery list="img/*" unique="true" cols=3 type="grid" gap="m" radius="true" zoom="true" hinode="false" >}}

## Masonry layout

{{< mgallery list="img/*" unique="true" cols=3 type="masonry" gap="m" radius="true" zoom="true" hinode="false" >}}
