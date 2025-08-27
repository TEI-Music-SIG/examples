# CETEIcean + Verovio + MathJax + SVG 📄🎵🎵➗📊

A minimal example to display TEI files with multiple sections of musical notation, **formulas** and **figures** within. Similar to [ceteicean-verovio](../ceteicean-verovio), but with additional TeX support using MathJax, plus native SVG support.

Live Demo: https://tei-music-sig.github.io/examples/ceteicean-verovio-mathjax-svg/

### How it works

- see [ceteicean-verovio](../ceteicean-verovio)
- a little JavaScript function manages the document selection
- MathJax is triggered when a `<formula>` element in TEI contains `@rend="tex"`.
- SVG is just rendered by the browser

### How to customize

- see [ceteicean-verovio](../ceteicean-verovio)

If you would like to display more than one TEI file, try [ceteicean-verovio-corpus](../ceteicean-verovio-corpus).
