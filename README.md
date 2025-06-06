# TEI/MEI Examples

This is a collection of examples, covering various usecases for MEI encoded music notation in TEI encoded text files.

## CETEIcean + Verovio

[ceteicean-verovio](ceteicean-verovio) contains a minimal example that allows using [CETEIcean](https://teic.github.io/CETEIcean) and [Verovio](https://www.verovio.org) together.

It requires only a simple webserver to work (e.g. GitHub Pages).

Live Demo: https://tei-music-sig.github.io/examples/ceteicean-verovio/

### How it works

- `index.html` includes CSS stylesheets, CETEIcean, Verovio and a TEI base file, and it manages the rendition process with a little JavaScript.
- TEI is rendered by CETEIcean. TEI files are kept separate in the `tei` folder.
- CETEIcean It prefixes all elements with `tei-` to make them directly styleable with CSS, without interfering with HTML.
- MEI is rendered by Verovio. MEI files are kept separately in the `mei` folder.
- Verovio is triggered when a `<notatedMusic>` element in TEI contains `@rend="MEI"` and `@xml:id` corresponds to a filename in `/mei` (without extension).

### How to customize

- Download the minimal example.
- Put your TEI document in the `tei` folder.
- Modify the stylesheet in `/css/custom.css` using `tei-*`
- Put your MEI snippets in the `mei` folder.
- Refer MEI files in the TEI by `<notatedMusic xml:id="[filename]" rend="MEI">`.
- Call `index.html` (or just the base directory) in your browser.

## CETEIcean + Verovio + Corpus

[ceteicean-verovio-corpus](ceteicean-verovio-corpus) contains everything above for multiple TEI documents.

Live Demo: https://tei-music-sig.github.io/examples/ceteicean-verovio-corpus/
