# CETEIcean + Verovio for one TEI file

A minimal example to display one TEI file with multiple sections of musical notation within.

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

If you would like to display more than one TEI file, try [ceteicean-verovio-corpus](ceteicean-verovio-corpus).
