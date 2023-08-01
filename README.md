# Hinode Module - mgallery

<!-- Tagline -->
<p align="center">
    <b>Create a gallery from a set of images in Hinode</b>
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
    <a href="https://github.com/myrthos/mod-mgallery/commits/main" alt="Last commit">
        <img src="https://img.shields.io/github/last-commit/gethinode/mod-template.svg">
    </a>
    <a href="https://github.com/myrthos/mod-mgallery/issues" alt="Issues">
        <img src="https://img.shields.io/github/issues/gethinode/mod-template.svg">
    </a>
    <a href="https://github.com/myrthos/mod-mgallery/pulls" alt="Pulls">
        <img src="https://img.shields.io/github/issues-pr-raw/gethinode/mod-template.svg">
    </a>
    <a href="https://github.com/myrthos/mod-mgallery/blob/main/LICENSE" alt="License">
        <img src="https://img.shields.io/github/license/gethinode/mod-template">
    </a>
</p>

## About

This module takes a set of images and creates a gallery from those images. The gallery can either be origanized in a grid or a vertical masonry. When an image is selected, a viewer opens, which is based on [Lightbox 2][lightbox].  
The module is intended to be used together with [Hinode](#hinode), a Hugo theme and, The module depends on Bootstrap, which is part of the Hinode theme.

To install this module in the Hinode theme, the following steps are needed:

1. Open the file `config/_default/hugo.toml` and add the following to the `[module]` section.

```toml
  [[module.imports]]
    path = "github.com/myrthos/mod-mgallery"
```

2. Open the file `config/_default/params.toml` and add the following to the `[modules]` section
    1. Add `, "mgallery` before the last bracket (`]`) of the `optional` parameter.
3. Run `npm run mod:update` from the command line, to download the latest version of the gallery. 

To use the gallery, the `mgallery` shortcode is used. On the page where this shortcode is used, the following should be part of the frontmatter:

```yaml
modules: ["mgallery"]
```

This will enable loading the required javascript files for the gallery.

## Hinode

Hinode is a clean blog theme for [Hugo][hugo], an open-source static site generator. Hinode is available as a [template][repository_template], and a [main theme][repository]. <!-- This repository maintains a Hugo module to add [module][module] to a Hinode site. --> Visit the Hinode documentation site for [installation instructions][hinode_docs].

<!-- MARKDOWN LINKS -->
[hugo]: https://gohugo.io
[hinode_docs]: https://gethinode.com
<!-- [module]: https://example.com -->
[repository]: https://github.com/gethinode/hinode.git
[repository_template]: https://github.com/gethinode/template.git
[lightbox]: https://lokeshdhakar.com/projects/lightbox2/
