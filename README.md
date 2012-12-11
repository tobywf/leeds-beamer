University of Leeds template for Beamer/LaTeX
=============================================

About
-----

This is a template for making presentations in Beamer. I have written a full custom theme which loosely adheres to the University of Leeds style guide and identity management rules.

Files
-----

- `beamerthemeLeeds.sty`
- `beamercolorthemeLeeds.sty`
- `beamercolorthemeLeedsBlack.sty`
- `beamercolorthemeLeedsGreen.sty`
- `beamercolorthemeLeedsRed.sty`
- `beamerfontthemeLeeds.sty`
- `beamerinnerthemeLeeds.sty`
- `beamerouterthemeLeeds.sty`
- `README.md`
- `Licence`
- `examples\colorschemes.pdf`
- `examples\colorschemes.tex`
- `examples\example.pdf`
- `examples\example.tex`
- `examples\LaTeX.png`

Most of these files are based on the themes that are distributed with Beamer by Till Tantau. Consequently -- like the original files -- they may be distributed and/or modified under the GNU Public License, specifically v3.

Licence
-------

see the file `LICENCE`.

Usage
-----

Simply place in your local `texmf` directory and add `\usetheme{Leeds}` to your beamer presentation.

FAQ
---

Q: Can I use the sub-themes ('color', 'font', 'inner', 'outer') separately?

A: Yes you can, e.g. you can use

	\usecolortheme{Leeds}
	\useoutertheme{sidebar}

to use the Leeds colours with the sidebar outer theme. The possibilities with the other themes are endless!

Q: How to I use the other colour themes?

A: Just include the main theme first, then the colour you want to use, e.g.:

	\usetheme{Leeds}
	\usecolortheme{LeedsRed}

Simple.

Q: Why does this not include the University of Leeds logo?

A: Because I'm not allowed to distribute it. Furthermore you need to get permission from the University to use it in any publication.

Q: What are the theme options?

A: There are several options, all which can be passed to the main theme or the appropriate sub-theme:

-	`height`: The height of the headline.

	Set to 0 to use the default headline template.
	Used by `beamerouterthemeLeeds`.

-	`logowidth`: The width of the logo container in the headline.

	Set to 0 to hide any logo, even if it is defined.
	Note: This will *NOT* rescale the logo to fit, it is merely the place allocated for the logo. The logo can overflow.
	Tip: Make this slightly bigger to give the logo some margins and space to be centred.
	Used by `beamerouterthemeLeeds`.

-	`nofootline`: Hide the footline.

	Used by `beamerouterthemeLeeds`.

-	`flat`: Use flat colours for structure elements (sidebars, headers, etc.).

	Used by `beamercolorthemeLeeds`.

-	`compress`: Tries to free up some extra space by compressing structure elements.

	In reality, this is left in for compatibility for switching from older themes and only reduces the text margins.
	Used by `beamerthemeLeeds`.

Q: Why does your FAQ not include more questions?

A: Because people haven't asked them!
