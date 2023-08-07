<!-- CSpell:ignore Hinode mgallery Lightbox shortcode frontmatter mgalleryblog -->
# Hinode Module - mgallery

<!-- Markdownlint-disable MD033 -->
<!-- Tagline -->
<p align="center">
    <b>Create a gallery from a set of images</b>
    <br />
</p>

<!-- Badges -->
<p align="center">
    <a href="https://gohugo.io" alt="Hugo website">
        <img src="https://img.shields.io/badge/generator-hugo-brightgreen">
    </a>
    <a href="https://gethinode.com" alt="Hinode theme">
        <img src="https://img.shields.io/badge/theme-hinode-blue">
    </a>
    <a href="https://github.com/myrthos/mod-mgallery/releases" alt="Last release">
        <img src="https://img.shields.io/github/v/release/myrthos/mod-mgallery">
    </a>
    <a href="https://github.com/myrthos/mod-mgallery/releases" alt="Release date">
        <img src="https://img.shields.io/github/release-date/myrthos/mod-mgallery">
    </a>
    <a href="https://github.com/myrthos/mod-mgallery/commits/main" alt="Last commit">
        <img src="https://img.shields.io/github/last-commit/myrthos/mod-mgallery/main">
    </a>
    <a href="https://github.com/myrthos/mod-mgallery/labels/bug" alt="bugs">
        <img src="https://img.shields.io/github/issues/myrthos/mod-mgallery/bug">
    </a>
    <a href="https://github.com/myrthos/mod-mgallery/blob/main/LICENSE" alt="License">
        <img src="https://img.shields.io/github/license/myrthos/mod-mgallery">
    </a>
</p>

## About

This module takes a set of images and creates a gallery from those images. The gallery can either be organized in a grid or a vertical masonry. When an image is selected, a viewer opens, which is based on [Lightbox 2][lightbox].  
The module is intended to be used together with [Hinode](#hinode), a Hugo theme. The module depends on Bootstrap, which is part of the Hinode theme.

## Installation

To install this module in a site using the Hinode theme, the following steps are needed on that site:

1. Open the file `config/_default/hugo.toml` and add the following to the `[module]` section.

```toml
  [[module.imports]]
    path = "github.com/myrthos/mod-mgallery"
```
<!-- Markdownlint-disable MD029 -->
2. Open the file `config/_default/params.toml` and add the following to the `[modules]` section  
   Add `, "mgallery"` before the last bracket (`]`) of the `optional` parameter.
3. Run `npm run mod:update` from the command line, to download the latest version of the gallery.
<!-- Markdownlint-enable MD029 -->

To use the gallery, the `mgallery` shortcode is used. On the page where this shortcode is used, the following should be part of the frontmatter:

```yaml
modules: ["mgallery"]
```

This will enable loading the required javascript files for the gallery.

## Documentation

For more information check the mgallery [blog][mgalleryblog] and [documentation][mgallerydoc]

## Hinode

Hinode is a clean blog theme for [Hugo][hugo], an open-source static site generator. Hinode is available as a [template][repository_template], and a [main theme][repository]. Visit the Hinode documentation site for [installation instructions][hinode_docs].

<!-- MARKDOWN LINKS -->
[hugo]: https://gohugo.io
[hinode_docs]: https://gethinode.com
[repository]: https://github.com/gethinode/hinode.git
[repository_template]: https://github.com/gethinode/template.git
[lightbox]: https://lokeshdhakar.com/projects/lightbox2/
[mgalleryblog]: https://myrthos.net/blog/mgallery/
[mgallerydoc]: https://myrthos.net/docs/shortcodes/mgallery/overview/
