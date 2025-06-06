# TEI/MEI Examples

This is a collection of examples, covering various scenarios for presenting sources that contain both text and music (in TEI and MEI respectively).

The example use common libraries [CETEIcean](https://teic.github.io/CETEIcean) and [Verovio](https://www.verovio.org) together. JavaScript is used to make them work together fluently. Hosting requirements are just a simple webserver (e.g. as provided by GitHub Pages, or local host).

## one TEI file + multiple MEI snippets

[ceteicean-verovio](ceteicean-verovio) contains a minimal example to display one TEI file with multiple sections of musical notation within.

## multiple TEI file + multiple MEI snippets

[ceteicean-verovio-corpus](ceteicean-verovio-corpus) works similarly to ceteicean-verovio, but for more than one TEI document.
