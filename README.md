# Foldit

[![][Fontbakery]](https://SophiaDesign.github.io/GF-Foldit/fontbakery-report.html)
[![][Universal]](https://SophiaDesign.github.io/GF-Foldit/fontbakery-report.html)
[![][GF Profile]](https://SophiaDesign.github.io/GF-Foldit/fontbakery-report.html)
[![][Outline Correctness]](https://SophiaDesign.github.io/GF-Foldit/fontbakery-report.html)
[![][Shaping]](https://SophiaDesign.github.io/GF-Foldit/fontbakery-report.html)

[Fontbakery]: https://img.shields.io/endpoint?url=https%3A%2F%2Fraw.githubusercontent.com%2FSophiaDesign%2FGF-Foldit%2Fgh-pages%2Fbadges%2Foverall.json
[GF Profile]: https://img.shields.io/endpoint?url=https%3A%2F%2Fraw.githubusercontent.com%2FSophiaDesign%2FGF-Foldit%2Fgh-pages%2Fbadges%2FGoogleFonts.json
[Outline Correctness]: https://img.shields.io/endpoint?url=https%3A%2F%2Fraw.githubusercontent.com%2FSophiaDesign%2FGF-Foldit%2Fgh-pages%2Fbadges%2FOutlineCorrectnessChecks.json
[Shaping]: https://img.shields.io/endpoint?url=https%3A%2F%2Fraw.githubusercontent.com%2FSophiaDesign%2FGF-Foldit%2Fgh-pages%2Fbadges%2FShapingChecks.json
[Universal]: https://img.shields.io/endpoint?url=https%3A%2F%2Fraw.githubusercontent.com%2FSophiaDesign%2FGF-Foldit%2Fgh-pages%2Fbadges%2FUniversal.json

Foldit is a COLRv1 variable font which uses gradients to play with dimension and sense of space. Styles run along weight and width axes with two masters: Thin Condensed and Extrabold Expanded. First version is available in GF Latin Plus character set. Concept of this design was, as the name suggest, based on a folded paper strip.

![Sample Image](documentation/image1.png)

## About

Sophia Tai ([@SophiaTypeLove](http://instagram.com/sophiatypelove)) is an independent typeface designer. She is a recipient of the 2021 Women of Typographic Excellence title and alumna of the MA Typeface Design course at University of Reading. 

Links: [website](http://www.sophiatai.com) | [github](https://github.com/SophiaDesign) | [instagram](http://instagram.com/sophiatypelove) | [twitter](http://twitter.com/sophiatypelove) | [twitch](http://twitch.tv/sophiatypelove)

## Building

Fonts are built automatically by GitHub Actions - take a look in the "Actions" tab for the latest build.

If you want to build fonts manually on your own computer:

* `make build` will produce font files.
* `make test` will run [FontBakery](https://github.com/googlefonts/fontbakery)'s quality assurance tests.
* `make proof` will generate HTML proof files.

The proof files and QA tests are also available automatically via GitHub Actions - look at `https://yourname.github.io/your-font-repository-name`.

## Changelog

When you update your font (new version or new release), please report all notable changes here, with a date.
[Font Versioning](https://github.com/googlefonts/gf-docs/tree/main/Spec#font-versioning) is based on semver. 
Changelog example:

**26 May 2021. Version 2.13**
- MAJOR Font turned to a variable font.
- SIGNIFICANT New Stylistic sets added.

## License

This Font Software is licensed under the SIL Open Font License, Version 1.1.
This license is copied below, and is also available with a FAQ at
https://scripts.sil.org/OFL

## Repository Layout

This font repository structure is inspired by [Unified Font Repository v0.3](https://github.com/unified-font-repository/Unified-Font-Repository), modified for the Google Fonts workflow.
