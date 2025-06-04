# TEI/MEI Examples

This is a collection of examples, covering various usecases for MEI encoded music notation in TEI encoded text files.

## CETEIcean and Verovio

[ceteicean-verovio](ceteicean-verovio) contains a minimal example that allows using [CETEIcean](https://teic.github.io/CETEIcean) and [Verovio](https://www.verovio.org) together. It requires a simple webserver to work.

**How to customize:** TEI elements are rendered by CETEIcean. The individual styles can be edited in `css/custom.css`. The music notation is kept in separate MEI files in the `mei`folder. The corresponding filenames in the TEI file are given in `@xml:id` of the `<notatedMusic>` elements. `@rend="MEI"` is a trigger to hand over renditioning from CETEIcean to Verovio.
