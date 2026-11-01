Fonts used for the headings of the website
==========================================
Instrument Sans (Regular 400, Bold 700), SIL Open Font License 1.1 - see InstrumentSans-OFL.txt.
The files are reduced to Latin characters (WOFF). Used in styles/common.scss (@font-face) and styles/light.scss / dark.scss ($headings-font-family).

To use a different heading font (e.g. Inter, a variable font, which also gives the weights 500/600):
  1. put the .woff2 file into this folder and keep its license text next to it,
  2. in styles/common.scss replace the two @font-face blocks (src: url("/fonts/<file>"), and for a variable font  font-weight: 100 900;),
  3. change the family name in $headings-font-family (styles/light.scss and styles/dark.scss) if you renamed it,
  4. set $headings-font-weight (light.scss / dark.scss) and the font-weight of .hero h1, .quarto-title h1.title, .stats strong to 500 or 600.
The path must start with /fonts/ (the css is stored in site_libs/, a relative path would not be found).
