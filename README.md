# AV-Hershey-Fonts

**This is a preliminary release, and most font files do not
  contain enough character glyphs for useful typesetting. As is, this
  distribution is _not yet_ recommended for the general user.**

A simple conversion of some subsets of the
“[Hershey fonts](https://en.wikipedia.org/wiki/Hershey_fonts)” to
OpenType format. All curves are approximated with short straight li segments.

## Files

Initially, the fonts keep the names inherited from AV-Hershey-OTF, but
these names don't match the data presented in [_Calligraphy for Computers_](https://archive.org/details/DTIC_AD0662398).
However, The upstream project references "tables" which aren't in the 
_Calligraphy for Computers_ paper, but appear to be referencing [_A Contribution to Computer Typesetting Techniques_](https://books.google.com/books?id=tGzop78ZCnMC), by Norman M. Wolcott, Joseph Hilsenrath of 
U.S. Department of Commerce, National Bureau of Standards, 1976. This work references Hershey as the source of the data. 
I have to research how universal this misnaming is, and come up with some
appropriate names that respect Hershey's work, yet more accurately describe
the contents. 

The point is, in this repo files are sorted into groups by font style, and
not by file type:

1. Simplex - FontForge and Source files that match the _Simplex FORTRAN Sans_
   outlines in Hershey's document. 

2. Duplex - FontForge and Source files that match the _Simplex Cartographic Sans_
   outlines in Hershey's document. Hershey seems to have assigned "simplex"
   to his outlines that had mono line thickness (Sans, and cursive).
   
3. Complex - Fontforge and Source files that match the _Duplex _  tree, but
   some glyphs are from the _Duplex Indexical_ coordinates, (g and other
   lower case), but some glyphes are from the _Duplex Principal_ coordinate list
   (numbers and most Capitals.)

A short reading of Hershey's document focused on classification yeilded this

1. **Simplex** - 1 line width (Sans fonts and ballpoint pen style cursive).

2. **Duplex** - Fonts with 2 strokes (major and minor strokes) styles and also including
   Serif fonts

3. **Complex** - Quill pen and eastern brush style calligraphy fonts. Hershey
   listed 3 faces in his repertory (English Gothic, Italian Gothic, and
   German Gothic), but also included "complex" Japanese calligraphic examples
   (Kanji and Hirigana) in an appendix.

Future revisions to this repo may rename files to respect Hershey's definitions
of the 3 levels of complexity.  If you read the text of the work, it's clearly
a major part of his paper. 

## Acknowledgements

* Derived from character stroke coordinates by Allen V. Hershey
  published in "Calligraphy for Computers" (US Naval Weapons
  Laboratory, 1967-08-01, NWL Report No. 2101, NTIS accession number
  AD-662 398) and elsewhere. These coordinates were published without
  copyright.

* The efforts of the Usenet Font Consortium (James Hurt, et al) who
  reformatted Hershey's data and published it to mod.sources on
  1986-04-01 [Volume 4, Issue 42] are greatly appreciated.

* On 2025/08/17, This repository was forked from the repo [AVHershey-OTF](https://github.com/scruss/AVHershey-OTF)
  by [Stewart C. Russell](http://scruss.com/blog/). Maybe some of the
  forked repo will survive into the Avante-Vangard fonts. 

## Todos

1. Migrate incoming data to appropriate font style names.  This may include separating
   the incoming data previously labelled 'duplex' into it's simplex and possibly duplex Sans
   sources.

2. Extract more font styles from the Hershey coordinate tables.

3. Fill in/expand characters to complete basic Latin unicode set.

4. Add basic accented characters.

5. Collect and publish a 'Hershey symbols' (or Hershey Dings?)  from the
   data he presented. 

## License

 CC0 1.0 Universal (see [COPYING](https://github.com/Avante-Vangard/AV-Hershey-Fonts/blob/master/COPYING).)
