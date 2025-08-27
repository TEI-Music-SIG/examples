# TEI/MEI Examples

This is a collection of examples, covering various scenarios for presenting sources that contain both text and music (in TEI and MEI respectively).

The examples use some common libraries together:

- [CETEIcean](https://teic.github.io/CETEIcean)
- [Verovio](https://www.verovio.org)
- [MathJax](https://www.mathjax.org)

Some extra JavaScript is used to make them work together fluently. Hosting requirements are just a simple webserver (e.g. as provided by GitHub Pages, or local host).

## one TEI file + multiple MEI snippets 📄🎵🎵

[ceteicean-verovio](ceteicean-verovio) contains a minimal example to display one TEI file with multiple sections of musical notation within.

## multiple TEI files + multiple MEI snippets 📄🎵🎵📄🎵🎵

[ceteicean-verovio-corpus](ceteicean-verovio-corpus) works similarly to ceteicean-verovio, but for more than one TEI document.

## one TEI file + multiple MEI snippets + TeX formulas 📄🎵🎵➗

[ceteicean-verovio-mathjax](ceteicean-verovio-mathjax) contains a minimal example to display one TEI file with multiple sections of musical notation within, plus multiple formulas.

## one TEI file + multiple MEI snippets + TeX formulas + SVG diagram 📄🎵🎵➗📊

[ceteicean-verovio-mathjax-svg](ceteicean-verovio-mathjax-svg) contains a minimal example to display one TEI file with multiple sections of musical notation within, plus multiple formulas and a diagram.
