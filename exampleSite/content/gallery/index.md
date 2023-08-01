<!-- Cspell:ignore ovlpos ovlx ovly ovlperc lightbox mgallery -->
<!-- markdownlint-disable MD003 MD022 MD041 -->
---
title: Gallery
description: Example for gallery
date: 2023-05-20
---
<!-- markdownlint-enable MD003 MD022 MD041 -->

To show this gallery properly in this example site, additional bootstrap classes are needed to wrap the gallery in.
It is still not exactly the same as when using Hinode, but close enough.

<div class="d-flex flex-column flex-fill">
    <div class="container-xxl">
        <div class="row row-cols-1">
            <div class="col col-sm-12 col-md-8">

## Grid layout

{{< mgallery list="img/*" unique="true" cols=3 type="grid" gap="m" radius="true" zoom="true" >}}

## Masonry layout

{{< mgallery list="img/*" unique="true" cols=3 type="masonry" gap="m" radius="true" zoom="true" >}}

</div>
</div>
</div>
</div>