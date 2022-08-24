## Fontbakery report

Fontbakery version: 0.8.9

<details><summary><b>[8] Foldit-Regular.ttf</b></summary><div><details><summary>💔 <b>ERROR:</b> Check Google Fonts glyph coverage. (<a href="https://font-bakery.readthedocs.io/en/stable/fontbakery/profiles/googlefonts.html#com.google.fonts/check/glyph_coverage">com.google.fonts/check/glyph_coverage</a>)</summary><div>


* 💔 **ERROR** Failed with IndexError: list index out of range
</div></details><details><summary>⚠ <b>WARN:</b> Is there kerning info for non-ligated sequences? (<a href="https://font-bakery.readthedocs.io/en/stable/fontbakery/profiles/googlefonts.html#com.google.fonts/check/kerning_for_non_ligated_sequences">com.google.fonts/check/kerning_for_non_ligated_sequences</a>)</summary><div>


* ⚠ **WARN** GPOS table lacks kerning info for the following non-ligated sequences:

	- f + f

	- f + i

	- i + f

	- f + l

	- l + f 

	- And i + l [code: lacks-kern-info]
</div></details><details><summary>⚠ <b>WARN:</b> Ensure fonts have ScriptLangTags declared on the 'meta' table. (<a href="https://font-bakery.readthedocs.io/en/stable/fontbakery/profiles/googlefonts.html#com.google.fonts/check/meta/script_lang_tags">com.google.fonts/check/meta/script_lang_tags</a>)</summary><div>


* ⚠ **WARN** This font file does not have a 'meta' table. [code: lacks-meta-table]
</div></details><details><summary>⚠ <b>WARN:</b> Check font contains no unreachable glyphs (<a href="https://font-bakery.readthedocs.io/en/stable/fontbakery/profiles/universal.html#com.google.fonts/check/unreachable_glyphs">com.google.fonts/check/unreachable_glyphs</a>)</summary><div>


* ⚠ **WARN** The following glyphs could not be reached by codepoint or substitution rules:

	- ccaron.color0

	- ordfeminine.color0

	- colonmonetary.color4

	- registered.color7

	- Ccedilla.color0

	- uni020D.color1

	- uni1EE4.color0

	- uni032E.color0

	- ampersand.color4

	- Edieresis.color1 

	- And 3012 more.

Use -F or --full-lists to disable shortening of long lists.
 [code: unreachable-glyphs]
</div></details><details><summary>⚠ <b>WARN:</b> Check if each glyph has the recommended amount of contours. (<a href="https://font-bakery.readthedocs.io/en/stable/fontbakery/profiles/universal.html#com.google.fonts/check/contour_count">com.google.fonts/check/contour_count</a>)</summary><div>


* ⚠ **WARN** This font has a 'Soft Hyphen' character (codepoint 0x00AD) which is supposed to be zero-width and invisible, and is used to mark a hyphenation possibility within a word in the absence of or overriding dictionary hyphenation. It is mostly an obsolete mechanism now, and the character is only included in fonts for legacy codepage coverage. [code: softhyphen]
* ⚠ **WARN** This check inspects the glyph outlines and detects the total number of contours in each of them. The expected values are infered from the typical ammounts of contours observed in a large collection of reference font families. The divergences listed below may simply indicate a significantly different design on some of your glyphs. On the other hand, some of these may flag actual bugs in the font such as glyphs mapped to an incorrect codepoint. Please consider reviewing the design and codepoint assignment of these to make sure they are correct.

The following glyphs do not have the recommended number of contours:

	- Glyph name: one	Contours detected: 2	Expected: 1

	- Glyph name: b	Contours detected: 1	Expected: 2

	- Glyph name: q	Contours detected: 1	Expected: 2

	- Glyph name: section	Contours detected: 1	Expected: 2

	- Glyph name: uni00AD	Contours detected: 1	Expected: 0

	- Glyph name: uni20A9	Contours detected: 6	Expected: 1, 3, 4 or 7

	- Glyph name: b	Contours detected: 1	Expected: 2

	- Glyph name: one	Contours detected: 2	Expected: 1

	- Glyph name: q	Contours detected: 1	Expected: 2

	- Glyph name: section	Contours detected: 1	Expected: 2

	- Glyph name: uni00AD	Contours detected: 1	Expected: 0 

	- And Glyph name: uni20A9	Contours detected: 6	Expected: 1, 3, 4 or 7
 [code: contour-count]
</div></details><details><summary>⚠ <b>WARN:</b> Ensure dotted circle glyph is present and can attach marks. (<a href="https://font-bakery.readthedocs.io/en/stable/fontbakery/profiles/universal.html#com.google.fonts/check/dotted_circle">com.google.fonts/check/dotted_circle</a>)</summary><div>


* ⚠ **WARN** No dotted circle glyph present [code: missing-dotted-circle]
</div></details><details><summary>⚠ <b>WARN:</b> Do outlines contain any jaggy segments? (<a href="https://font-bakery.readthedocs.io/en/stable/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_jaggy_segments">com.google.fonts/check/outline_jaggy_segments</a>)</summary><div>


* ⚠ **WARN** The following glyphs have jaggy segments:

	* colonmonetary (U+20A1): L<<137.0,623.0>--<137.0,100.0>>/L<<137.0,100.0>--<212.0,623.0>> = 8.160774610065934 [code: found-jaggy-segments]
</div></details><details><summary>⚠ <b>WARN:</b> Do outlines contain any semi-vertical or semi-horizontal lines? (<a href="https://font-bakery.readthedocs.io/en/stable/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_semi_vertical">com.google.fonts/check/outline_semi_vertical</a>)</summary><div>


* ⚠ **WARN** The following glyphs have semi-vertical/semi-horizontal lines:

	* M (U+004D): L<<593.0,702.0>--<590.0,0.0>>

	* b (U+0062): L<<134.0,748.0>--<135.0,85.0>>

	* dollar (U+0024): L<<260.0,328.0>--<261.0,85.0>>

	* franc (U+20A3): L<<265.0,170.0>--<150.0,169.0>>

	* plusminus (U+00B1): L<<373.0,171.0>--<45.0,170.0>>

	* q (U+0071): L<<256.0,-200.0>--<255.0,343.0>>

	* sterling (U+00A3): L<<447.0,349.0>--<200.0,348.0>>

	* trademark (U+2122): L<<472.0,442.0>--<471.0,618.0>>

	* uni20BC (U+20BC): L<<182.0,77.0>--<181.0,623.0>>

	* uni20BC (U+20BC): L<<263.0,623.0>--<264.0,100.0>>

	* yen (U+00A5): L<<33.0,247.0>--<166.0,248.0>> 

	* And yen (U+00A5): L<<33.0,336.0>--<164.0,337.0>> [code: found-semi-vertical]
</div></details><br></div></details><details><summary><b>[9] Foldit-Thin.ttf</b></summary><div><details><summary>💔 <b>ERROR:</b> Check Google Fonts glyph coverage. (<a href="https://font-bakery.readthedocs.io/en/stable/fontbakery/profiles/googlefonts.html#com.google.fonts/check/glyph_coverage">com.google.fonts/check/glyph_coverage</a>)</summary><div>


* 💔 **ERROR** Failed with IndexError: list index out of range
</div></details><details><summary>⚠ <b>WARN:</b> Is there kerning info for non-ligated sequences? (<a href="https://font-bakery.readthedocs.io/en/stable/fontbakery/profiles/googlefonts.html#com.google.fonts/check/kerning_for_non_ligated_sequences">com.google.fonts/check/kerning_for_non_ligated_sequences</a>)</summary><div>


* ⚠ **WARN** GPOS table lacks kerning info for the following non-ligated sequences:

	- f + f

	- f + i

	- i + f

	- f + l

	- l + f 

	- And i + l [code: lacks-kern-info]
</div></details><details><summary>⚠ <b>WARN:</b> Ensure fonts have ScriptLangTags declared on the 'meta' table. (<a href="https://font-bakery.readthedocs.io/en/stable/fontbakery/profiles/googlefonts.html#com.google.fonts/check/meta/script_lang_tags">com.google.fonts/check/meta/script_lang_tags</a>)</summary><div>


* ⚠ **WARN** This font file does not have a 'meta' table. [code: lacks-meta-table]
</div></details><details><summary>⚠ <b>WARN:</b> Check font contains no unreachable glyphs (<a href="https://font-bakery.readthedocs.io/en/stable/fontbakery/profiles/universal.html#com.google.fonts/check/unreachable_glyphs">com.google.fonts/check/unreachable_glyphs</a>)</summary><div>


* ⚠ **WARN** The following glyphs could not be reached by codepoint or substitution rules:

	- ccaron.color0

	- ordfeminine.color0

	- colonmonetary.color4

	- registered.color7

	- Ccedilla.color0

	- uni020D.color1

	- uni1EE4.color0

	- uni032E.color0

	- ampersand.color4

	- Edieresis.color1 

	- And 3012 more.

Use -F or --full-lists to disable shortening of long lists.
 [code: unreachable-glyphs]
</div></details><details><summary>⚠ <b>WARN:</b> Check if each glyph has the recommended amount of contours. (<a href="https://font-bakery.readthedocs.io/en/stable/fontbakery/profiles/universal.html#com.google.fonts/check/contour_count">com.google.fonts/check/contour_count</a>)</summary><div>


* ⚠ **WARN** This font has a 'Soft Hyphen' character (codepoint 0x00AD) which is supposed to be zero-width and invisible, and is used to mark a hyphenation possibility within a word in the absence of or overriding dictionary hyphenation. It is mostly an obsolete mechanism now, and the character is only included in fonts for legacy codepage coverage. [code: softhyphen]
* ⚠ **WARN** This check inspects the glyph outlines and detects the total number of contours in each of them. The expected values are infered from the typical ammounts of contours observed in a large collection of reference font families. The divergences listed below may simply indicate a significantly different design on some of your glyphs. On the other hand, some of these may flag actual bugs in the font such as glyphs mapped to an incorrect codepoint. Please consider reviewing the design and codepoint assignment of these to make sure they are correct.

The following glyphs do not have the recommended number of contours:

	- Glyph name: at	Contours detected: 1	Expected: 2

	- Glyph name: uni00AD	Contours detected: 1	Expected: 0

	- Glyph name: at	Contours detected: 1	Expected: 2 

	- And Glyph name: uni00AD	Contours detected: 1	Expected: 0
 [code: contour-count]
</div></details><details><summary>⚠ <b>WARN:</b> Ensure dotted circle glyph is present and can attach marks. (<a href="https://font-bakery.readthedocs.io/en/stable/fontbakery/profiles/universal.html#com.google.fonts/check/dotted_circle">com.google.fonts/check/dotted_circle</a>)</summary><div>


* ⚠ **WARN** No dotted circle glyph present [code: missing-dotted-circle]
</div></details><details><summary>⚠ <b>WARN:</b> Do any segments have colinear vectors? (<a href="https://font-bakery.readthedocs.io/en/stable/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_colinear_vectors">com.google.fonts/check/outline_colinear_vectors</a>)</summary><div>


* ⚠ **WARN** The following glyphs have colinear vectors:

	* Abreve (U+0102): L<<110.0,781.0>--<91.0,803.0>> -> L<<91.0,803.0>--<60.0,839.0>>

	* Abreve (U+0102): L<<216.0,839.0>--<185.0,803.0>> -> L<<185.0,803.0>--<166.0,781.0>>

	* Ebreve (U+0114): L<<110.0,781.0>--<91.0,803.0>> -> L<<91.0,803.0>--<60.0,839.0>>

	* Ebreve (U+0114): L<<216.0,839.0>--<185.0,803.0>> -> L<<185.0,803.0>--<166.0,781.0>>

	* Gbreve (U+011E): L<<110.0,781.0>--<91.0,803.0>> -> L<<91.0,803.0>--<60.0,839.0>>

	* Gbreve (U+011E): L<<216.0,839.0>--<185.0,803.0>> -> L<<185.0,803.0>--<166.0,781.0>>

	* Ibreve (U+012C): L<<193.0,839.0>--<162.0,803.0>> -> L<<162.0,803.0>--<143.0,781.0>>

	* Ibreve (U+012C): L<<87.0,781.0>--<68.0,803.0>> -> L<<68.0,803.0>--<37.0,839.0>>

	* Lcaron (U+013D): L<<151.0,700.0>--<151.0,699.0>> -> L<<151.0,699.0>--<146.0,570.0>>

	* M (U+004D): L<<343.0,703.0>--<356.0,695.0>> -> L<<356.0,695.0>--<365.0,690.0>> 

	* And 73 more.

Use -F or --full-lists to disable shortening of long lists. [code: found-colinear-vectors]
</div></details><details><summary>⚠ <b>WARN:</b> Do outlines contain any jaggy segments? (<a href="https://font-bakery.readthedocs.io/en/stable/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_jaggy_segments">com.google.fonts/check/outline_jaggy_segments</a>)</summary><div>


* ⚠ **WARN** The following glyphs have jaggy segments:

	* M (U+004D): L<<197.0,-3.0>--<77.0,582.0>>/L<<77.0,582.0>--<77.0,0.0>> = 11.592175410291073

	* M (U+004D): L<<342.0,0.0>--<342.0,579.0>>/L<<342.0,579.0>--<221.0,-3.0>> = 11.744699097555973

	* V (U+0056): L<<47.0,700.0>--<119.0,98.0>>/L<<119.0,98.0>--<183.0,700.0>> = 12.888706108187892

	* colonmonetary (U+20A1): L<<82.0,676.0>--<82.0,377.0>>/L<<82.0,377.0>--<116.0,676.0>> = 6.4873732411041445

	* oslash (U+00F8): L<<124.0,24.0>--<124.0,301.0>>/L<<124.0,301.0>--<74.0,86.0>> = 13.091893064346833

	* oslash (U+00F8): L<<74.0,476.0>--<74.0,177.0>>/L<<74.0,177.0>--<124.0,392.0>> = 13.091893064346833

	* oslashacute (U+01FF): L<<124.0,24.0>--<124.0,301.0>>/L<<124.0,301.0>--<74.0,86.0>> = 13.091893064346833

	* oslashacute (U+01FF): L<<74.0,476.0>--<74.0,177.0>>/L<<74.0,177.0>--<124.0,392.0>> = 13.091893064346833

	* zero (U+0030): L<<200.0,24.0>--<77.0,618.0>>/L<<77.0,618.0>--<77.0,24.0>> = 11.698937608802657 

	* And zero (U+0030): L<<94.0,646.0>--<213.0,73.0>>/L<<213.0,73.0>--<213.0,646.0>> = 11.732346787462378 [code: found-jaggy-segments]
</div></details><details><summary>⚠ <b>WARN:</b> Do outlines contain any semi-vertical or semi-horizontal lines? (<a href="https://font-bakery.readthedocs.io/en/stable/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_semi_vertical">com.google.fonts/check/outline_semi_vertical</a>)</summary><div>


* ⚠ **WARN** The following glyphs have semi-vertical/semi-horizontal lines:

	* Euro (U+20AC): L<<132.0,353.0>--<252.0,354.0>>

	* Euro (U+20AC): L<<132.0,442.0>--<252.0,443.0>>

	* Euro (U+20AC): L<<275.0,330.0>--<132.0,329.0>>

	* Euro (U+20AC): L<<275.0,419.0>--<132.0,418.0>>

	* dollar (U+0024): L<<114.0,24.0>--<113.0,353.0>>

	* g (U+0067): L<<147.0,476.0>--<146.0,-177.0>>

	* gbreve (U+011F): L<<147.0,476.0>--<146.0,-177.0>>

	* gcaron (U+01E7): L<<147.0,476.0>--<146.0,-177.0>>

	* gcircumflex (U+011D): L<<147.0,476.0>--<146.0,-177.0>>

	* gdotaccent (U+0121): L<<147.0,476.0>--<146.0,-177.0>> 

	* And 17 more.

Use -F or --full-lists to disable shortening of long lists. [code: found-semi-vertical]
</div></details><br></div></details><details><summary><b>[7] Foldit-SemiBold.ttf</b></summary><div><details><summary>💔 <b>ERROR:</b> Check Google Fonts glyph coverage. (<a href="https://font-bakery.readthedocs.io/en/stable/fontbakery/profiles/googlefonts.html#com.google.fonts/check/glyph_coverage">com.google.fonts/check/glyph_coverage</a>)</summary><div>


* 💔 **ERROR** Failed with IndexError: list index out of range
</div></details><details><summary>⚠ <b>WARN:</b> Is there kerning info for non-ligated sequences? (<a href="https://font-bakery.readthedocs.io/en/stable/fontbakery/profiles/googlefonts.html#com.google.fonts/check/kerning_for_non_ligated_sequences">com.google.fonts/check/kerning_for_non_ligated_sequences</a>)</summary><div>


* ⚠ **WARN** GPOS table lacks kerning info for the following non-ligated sequences:

	- f + f

	- f + i

	- i + f

	- f + l

	- l + f 

	- And i + l [code: lacks-kern-info]
</div></details><details><summary>⚠ <b>WARN:</b> Ensure fonts have ScriptLangTags declared on the 'meta' table. (<a href="https://font-bakery.readthedocs.io/en/stable/fontbakery/profiles/googlefonts.html#com.google.fonts/check/meta/script_lang_tags">com.google.fonts/check/meta/script_lang_tags</a>)</summary><div>


* ⚠ **WARN** This font file does not have a 'meta' table. [code: lacks-meta-table]
</div></details><details><summary>⚠ <b>WARN:</b> Check font contains no unreachable glyphs (<a href="https://font-bakery.readthedocs.io/en/stable/fontbakery/profiles/universal.html#com.google.fonts/check/unreachable_glyphs">com.google.fonts/check/unreachable_glyphs</a>)</summary><div>


* ⚠ **WARN** The following glyphs could not be reached by codepoint or substitution rules:

	- ccaron.color0

	- ordfeminine.color0

	- colonmonetary.color4

	- registered.color7

	- Ccedilla.color0

	- uni020D.color1

	- uni1EE4.color0

	- uni032E.color0

	- ampersand.color4

	- Edieresis.color1 

	- And 3012 more.

Use -F or --full-lists to disable shortening of long lists.
 [code: unreachable-glyphs]
</div></details><details><summary>⚠ <b>WARN:</b> Check if each glyph has the recommended amount of contours. (<a href="https://font-bakery.readthedocs.io/en/stable/fontbakery/profiles/universal.html#com.google.fonts/check/contour_count">com.google.fonts/check/contour_count</a>)</summary><div>


* ⚠ **WARN** This font has a 'Soft Hyphen' character (codepoint 0x00AD) which is supposed to be zero-width and invisible, and is used to mark a hyphenation possibility within a word in the absence of or overriding dictionary hyphenation. It is mostly an obsolete mechanism now, and the character is only included in fonts for legacy codepage coverage. [code: softhyphen]
* ⚠ **WARN** This check inspects the glyph outlines and detects the total number of contours in each of them. The expected values are infered from the typical ammounts of contours observed in a large collection of reference font families. The divergences listed below may simply indicate a significantly different design on some of your glyphs. On the other hand, some of these may flag actual bugs in the font such as glyphs mapped to an incorrect codepoint. Please consider reviewing the design and codepoint assignment of these to make sure they are correct.

The following glyphs do not have the recommended number of contours:

	- Glyph name: one	Contours detected: 2	Expected: 1

	- Glyph name: b	Contours detected: 1	Expected: 2

	- Glyph name: q	Contours detected: 1	Expected: 2

	- Glyph name: uni00AD	Contours detected: 1	Expected: 0

	- Glyph name: uni20A6	Contours detected: 4	Expected: 1, 3 or 5

	- Glyph name: uni20A9	Contours detected: 5	Expected: 1, 3, 4 or 7

	- Glyph name: b	Contours detected: 1	Expected: 2

	- Glyph name: one	Contours detected: 2	Expected: 1

	- Glyph name: q	Contours detected: 1	Expected: 2

	- Glyph name: uni00AD	Contours detected: 1	Expected: 0

	- Glyph name: uni20A6	Contours detected: 4	Expected: 1, 3 or 5 

	- And Glyph name: uni20A9	Contours detected: 5	Expected: 1, 3, 4 or 7
 [code: contour-count]
</div></details><details><summary>⚠ <b>WARN:</b> Ensure dotted circle glyph is present and can attach marks. (<a href="https://font-bakery.readthedocs.io/en/stable/fontbakery/profiles/universal.html#com.google.fonts/check/dotted_circle">com.google.fonts/check/dotted_circle</a>)</summary><div>


* ⚠ **WARN** No dotted circle glyph present [code: missing-dotted-circle]
</div></details><details><summary>⚠ <b>WARN:</b> Do outlines contain any semi-vertical or semi-horizontal lines? (<a href="https://font-bakery.readthedocs.io/en/stable/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_semi_vertical">com.google.fonts/check/outline_semi_vertical</a>)</summary><div>


* ⚠ **WARN** The following glyphs have semi-vertical/semi-horizontal lines:

	* M (U+004D): L<<755.0,711.0>--<751.0,0.0>>

	* dollar (U+0024): L<<348.0,309.0>--<349.0,129.0>>

	* franc (U+20A3): L<<327.0,156.0>--<192.0,155.0>>

	* g (U+0067): L<<471.0,385.0>--<470.0,-142.0>>

	* gbreve (U+011F): L<<471.0,385.0>--<470.0,-142.0>>

	* gcaron (U+01E7): L<<471.0,385.0>--<470.0,-142.0>>

	* gcircumflex (U+011D): L<<471.0,385.0>--<470.0,-142.0>>

	* gdotaccent (U+0121): L<<471.0,385.0>--<470.0,-142.0>>

	* greaterequal (U+2265): L<<466.0,112.0>--<40.0,113.0>>

	* k (U+006B): L<<176.0,761.0>--<177.0,0.0>> 

	* And 26 more.

Use -F or --full-lists to disable shortening of long lists. [code: found-semi-vertical]
</div></details><br></div></details><details><summary><b>[8] Foldit-ExtraLight.ttf</b></summary><div><details><summary>💔 <b>ERROR:</b> Check Google Fonts glyph coverage. (<a href="https://font-bakery.readthedocs.io/en/stable/fontbakery/profiles/googlefonts.html#com.google.fonts/check/glyph_coverage">com.google.fonts/check/glyph_coverage</a>)</summary><div>


* 💔 **ERROR** Failed with IndexError: list index out of range
</div></details><details><summary>⚠ <b>WARN:</b> Is there kerning info for non-ligated sequences? (<a href="https://font-bakery.readthedocs.io/en/stable/fontbakery/profiles/googlefonts.html#com.google.fonts/check/kerning_for_non_ligated_sequences">com.google.fonts/check/kerning_for_non_ligated_sequences</a>)</summary><div>


* ⚠ **WARN** GPOS table lacks kerning info for the following non-ligated sequences:

	- f + f

	- f + i

	- i + f

	- f + l

	- l + f 

	- And i + l [code: lacks-kern-info]
</div></details><details><summary>⚠ <b>WARN:</b> Ensure fonts have ScriptLangTags declared on the 'meta' table. (<a href="https://font-bakery.readthedocs.io/en/stable/fontbakery/profiles/googlefonts.html#com.google.fonts/check/meta/script_lang_tags">com.google.fonts/check/meta/script_lang_tags</a>)</summary><div>


* ⚠ **WARN** This font file does not have a 'meta' table. [code: lacks-meta-table]
</div></details><details><summary>⚠ <b>WARN:</b> Check font contains no unreachable glyphs (<a href="https://font-bakery.readthedocs.io/en/stable/fontbakery/profiles/universal.html#com.google.fonts/check/unreachable_glyphs">com.google.fonts/check/unreachable_glyphs</a>)</summary><div>


* ⚠ **WARN** The following glyphs could not be reached by codepoint or substitution rules:

	- ccaron.color0

	- ordfeminine.color0

	- colonmonetary.color4

	- registered.color7

	- Ccedilla.color0

	- uni020D.color1

	- uni1EE4.color0

	- uni032E.color0

	- ampersand.color4

	- Edieresis.color1 

	- And 3012 more.

Use -F or --full-lists to disable shortening of long lists.
 [code: unreachable-glyphs]
</div></details><details><summary>⚠ <b>WARN:</b> Check if each glyph has the recommended amount of contours. (<a href="https://font-bakery.readthedocs.io/en/stable/fontbakery/profiles/universal.html#com.google.fonts/check/contour_count">com.google.fonts/check/contour_count</a>)</summary><div>


* ⚠ **WARN** This font has a 'Soft Hyphen' character (codepoint 0x00AD) which is supposed to be zero-width and invisible, and is used to mark a hyphenation possibility within a word in the absence of or overriding dictionary hyphenation. It is mostly an obsolete mechanism now, and the character is only included in fonts for legacy codepage coverage. [code: softhyphen]
* ⚠ **WARN** This check inspects the glyph outlines and detects the total number of contours in each of them. The expected values are infered from the typical ammounts of contours observed in a large collection of reference font families. The divergences listed below may simply indicate a significantly different design on some of your glyphs. On the other hand, some of these may flag actual bugs in the font such as glyphs mapped to an incorrect codepoint. Please consider reviewing the design and codepoint assignment of these to make sure they are correct.

The following glyphs do not have the recommended number of contours:

	- Glyph name: one	Contours detected: 2	Expected: 1

	- Glyph name: b	Contours detected: 1	Expected: 2

	- Glyph name: q	Contours detected: 1	Expected: 2

	- Glyph name: uni00AD	Contours detected: 1	Expected: 0

	- Glyph name: b	Contours detected: 1	Expected: 2

	- Glyph name: one	Contours detected: 2	Expected: 1

	- Glyph name: q	Contours detected: 1	Expected: 2 

	- And Glyph name: uni00AD	Contours detected: 1	Expected: 0
 [code: contour-count]
</div></details><details><summary>⚠ <b>WARN:</b> Ensure dotted circle glyph is present and can attach marks. (<a href="https://font-bakery.readthedocs.io/en/stable/fontbakery/profiles/universal.html#com.google.fonts/check/dotted_circle">com.google.fonts/check/dotted_circle</a>)</summary><div>


* ⚠ **WARN** No dotted circle glyph present [code: missing-dotted-circle]
</div></details><details><summary>⚠ <b>WARN:</b> Do outlines contain any jaggy segments? (<a href="https://font-bakery.readthedocs.io/en/stable/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_jaggy_segments">com.google.fonts/check/outline_jaggy_segments</a>)</summary><div>


* ⚠ **WARN** The following glyphs have jaggy segments:

	* M (U+004D): L<<210.0,-3.0>--<87.0,545.0>>/L<<87.0,545.0>--<87.0,0.0>> = 12.650525095506046

	* M (U+004D): L<<369.0,0.0>--<369.0,558.0>>/L<<369.0,558.0>--<245.0,-3.0>> = 12.463907854506944

	* colonmonetary (U+20A1): L<<91.0,667.0>--<91.0,320.0>>/L<<91.0,320.0>--<133.0,667.0>> = 6.9013646904254555

	* zero (U+0030): L<<109.0,638.0>--<228.0,104.0>>/L<<228.0,104.0>--<228.0,638.0>> = 12.56288529009344 

	* And zero (U+0030): L<<211.0,35.0>--<87.0,596.0>>/L<<87.0,596.0>--<87.0,35.0>> = 12.463907854506944 [code: found-jaggy-segments]
</div></details><details><summary>⚠ <b>WARN:</b> Do outlines contain any semi-vertical or semi-horizontal lines? (<a href="https://font-bakery.readthedocs.io/en/stable/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_semi_vertical">com.google.fonts/check/outline_semi_vertical</a>)</summary><div>


* ⚠ **WARN** The following glyphs have semi-vertical/semi-horizontal lines:

	* Euro (U+20AC): L<<142.0,352.0>--<279.0,353.0>>

	* Euro (U+20AC): L<<142.0,441.0>--<279.0,442.0>>

	* Euro (U+20AC): L<<302.0,329.0>--<142.0,328.0>>

	* Euro (U+20AC): L<<302.0,418.0>--<142.0,417.0>>

	* Lcaron (U+013D): L<<136.0,570.0>--<135.0,704.0>>

	* M (U+004D): L<<405.0,691.0>--<404.0,0.0>>

	* dcaron (U+010F): L<<213.0,599.0>--<212.0,733.0>>

	* dollar (U+0024): L<<125.0,381.0>--<124.0,667.0>>

	* dollar (U+0024): L<<158.0,667.0>--<159.0,381.0>>

	* g (U+0067): L<<179.0,467.0>--<178.0,-174.0>> 

	* And 24 more.

Use -F or --full-lists to disable shortening of long lists. [code: found-semi-vertical]
</div></details><br></div></details><details><summary><b>[8] Foldit-Light.ttf</b></summary><div><details><summary>💔 <b>ERROR:</b> Check Google Fonts glyph coverage. (<a href="https://font-bakery.readthedocs.io/en/stable/fontbakery/profiles/googlefonts.html#com.google.fonts/check/glyph_coverage">com.google.fonts/check/glyph_coverage</a>)</summary><div>


* 💔 **ERROR** Failed with IndexError: list index out of range
</div></details><details><summary>⚠ <b>WARN:</b> Is there kerning info for non-ligated sequences? (<a href="https://font-bakery.readthedocs.io/en/stable/fontbakery/profiles/googlefonts.html#com.google.fonts/check/kerning_for_non_ligated_sequences">com.google.fonts/check/kerning_for_non_ligated_sequences</a>)</summary><div>


* ⚠ **WARN** GPOS table lacks kerning info for the following non-ligated sequences:

	- f + f

	- f + i

	- i + f

	- f + l

	- l + f 

	- And i + l [code: lacks-kern-info]
</div></details><details><summary>⚠ <b>WARN:</b> Ensure fonts have ScriptLangTags declared on the 'meta' table. (<a href="https://font-bakery.readthedocs.io/en/stable/fontbakery/profiles/googlefonts.html#com.google.fonts/check/meta/script_lang_tags">com.google.fonts/check/meta/script_lang_tags</a>)</summary><div>


* ⚠ **WARN** This font file does not have a 'meta' table. [code: lacks-meta-table]
</div></details><details><summary>⚠ <b>WARN:</b> Check font contains no unreachable glyphs (<a href="https://font-bakery.readthedocs.io/en/stable/fontbakery/profiles/universal.html#com.google.fonts/check/unreachable_glyphs">com.google.fonts/check/unreachable_glyphs</a>)</summary><div>


* ⚠ **WARN** The following glyphs could not be reached by codepoint or substitution rules:

	- ccaron.color0

	- ordfeminine.color0

	- colonmonetary.color4

	- registered.color7

	- Ccedilla.color0

	- uni020D.color1

	- uni1EE4.color0

	- uni032E.color0

	- ampersand.color4

	- Edieresis.color1 

	- And 3012 more.

Use -F or --full-lists to disable shortening of long lists.
 [code: unreachable-glyphs]
</div></details><details><summary>⚠ <b>WARN:</b> Check if each glyph has the recommended amount of contours. (<a href="https://font-bakery.readthedocs.io/en/stable/fontbakery/profiles/universal.html#com.google.fonts/check/contour_count">com.google.fonts/check/contour_count</a>)</summary><div>


* ⚠ **WARN** This font has a 'Soft Hyphen' character (codepoint 0x00AD) which is supposed to be zero-width and invisible, and is used to mark a hyphenation possibility within a word in the absence of or overriding dictionary hyphenation. It is mostly an obsolete mechanism now, and the character is only included in fonts for legacy codepage coverage. [code: softhyphen]
* ⚠ **WARN** This check inspects the glyph outlines and detects the total number of contours in each of them. The expected values are infered from the typical ammounts of contours observed in a large collection of reference font families. The divergences listed below may simply indicate a significantly different design on some of your glyphs. On the other hand, some of these may flag actual bugs in the font such as glyphs mapped to an incorrect codepoint. Please consider reviewing the design and codepoint assignment of these to make sure they are correct.

The following glyphs do not have the recommended number of contours:

	- Glyph name: one	Contours detected: 2	Expected: 1

	- Glyph name: b	Contours detected: 1	Expected: 2

	- Glyph name: q	Contours detected: 1	Expected: 2

	- Glyph name: uni00AD	Contours detected: 1	Expected: 0

	- Glyph name: b	Contours detected: 1	Expected: 2

	- Glyph name: one	Contours detected: 2	Expected: 1

	- Glyph name: q	Contours detected: 1	Expected: 2 

	- And Glyph name: uni00AD	Contours detected: 1	Expected: 0
 [code: contour-count]
</div></details><details><summary>⚠ <b>WARN:</b> Ensure dotted circle glyph is present and can attach marks. (<a href="https://font-bakery.readthedocs.io/en/stable/fontbakery/profiles/universal.html#com.google.fonts/check/dotted_circle">com.google.fonts/check/dotted_circle</a>)</summary><div>


* ⚠ **WARN** No dotted circle glyph present [code: missing-dotted-circle]
</div></details><details><summary>⚠ <b>WARN:</b> Do outlines contain any jaggy segments? (<a href="https://font-bakery.readthedocs.io/en/stable/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_jaggy_segments">com.google.fonts/check/outline_jaggy_segments</a>)</summary><div>


* ⚠ **WARN** The following glyphs have jaggy segments:

	* M (U+004D): L<<422.0,0.0>--<422.0,522.0>>/L<<422.0,522.0>--<292.0,-3.0>> = 13.907777809854704

	* colonmonetary (U+20A1): L<<109.0,650.0>--<109.0,222.0>>/L<<109.0,222.0>--<164.0,650.0>> = 7.322644008425584

	* zero (U+0030): L<<137.0,624.0>--<256.0,156.0>>/L<<256.0,156.0>--<256.0,624.0>> = 14.266461332998118 

	* And zero (U+0030): L<<233.0,55.0>--<105.0,560.0>>/L<<105.0,560.0>--<105.0,55.0>> = 14.222960896604942 [code: found-jaggy-segments]
</div></details><details><summary>⚠ <b>WARN:</b> Do outlines contain any semi-vertical or semi-horizontal lines? (<a href="https://font-bakery.readthedocs.io/en/stable/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_semi_vertical">com.google.fonts/check/outline_semi_vertical</a>)</summary><div>


* ⚠ **WARN** The following glyphs have semi-vertical/semi-horizontal lines:

	* G (U+0047): L<<147.0,389.0>--<270.0,390.0>>

	* Gbreve (U+011E): L<<147.0,389.0>--<270.0,390.0>>

	* Gcaron (U+01E6): L<<147.0,389.0>--<270.0,390.0>>

	* Gcircumflex (U+011C): L<<147.0,389.0>--<270.0,390.0>>

	* Gdotaccent (U+0120): L<<147.0,389.0>--<270.0,390.0>>

	* M (U+004D): L<<479.0,696.0>--<478.0,0.0>>

	* T (U+0054): L<<166.0,0.0>--<167.0,650.0>>

	* Tbar (U+0166): L<<166.0,388.0>--<167.0,650.0>>

	* Tcaron (U+0164): L<<166.0,0.0>--<167.0,650.0>>

	* dollar (U+0024): L<<146.0,389.0>--<145.0,650.0>> 

	* And 31 more.

Use -F or --full-lists to disable shortening of long lists. [code: found-semi-vertical]
</div></details><br></div></details><details><summary><b>[8] Foldit-ExtraBold.ttf</b></summary><div><details><summary>💔 <b>ERROR:</b> Check Google Fonts glyph coverage. (<a href="https://font-bakery.readthedocs.io/en/stable/fontbakery/profiles/googlefonts.html#com.google.fonts/check/glyph_coverage">com.google.fonts/check/glyph_coverage</a>)</summary><div>


* 💔 **ERROR** Failed with IndexError: list index out of range
</div></details><details><summary>⚠ <b>WARN:</b> Is there kerning info for non-ligated sequences? (<a href="https://font-bakery.readthedocs.io/en/stable/fontbakery/profiles/googlefonts.html#com.google.fonts/check/kerning_for_non_ligated_sequences">com.google.fonts/check/kerning_for_non_ligated_sequences</a>)</summary><div>


* ⚠ **WARN** GPOS table lacks kerning info for the following non-ligated sequences:

	- f + f

	- f + i

	- i + f

	- f + l

	- l + f 

	- And i + l [code: lacks-kern-info]
</div></details><details><summary>⚠ <b>WARN:</b> Ensure fonts have ScriptLangTags declared on the 'meta' table. (<a href="https://font-bakery.readthedocs.io/en/stable/fontbakery/profiles/googlefonts.html#com.google.fonts/check/meta/script_lang_tags">com.google.fonts/check/meta/script_lang_tags</a>)</summary><div>


* ⚠ **WARN** This font file does not have a 'meta' table. [code: lacks-meta-table]
</div></details><details><summary>⚠ <b>WARN:</b> Check font contains no unreachable glyphs (<a href="https://font-bakery.readthedocs.io/en/stable/fontbakery/profiles/universal.html#com.google.fonts/check/unreachable_glyphs">com.google.fonts/check/unreachable_glyphs</a>)</summary><div>


* ⚠ **WARN** The following glyphs could not be reached by codepoint or substitution rules:

	- ccaron.color0

	- ordfeminine.color0

	- colonmonetary.color4

	- registered.color7

	- Ccedilla.color0

	- uni020D.color1

	- uni1EE4.color0

	- uni032E.color0

	- ampersand.color4

	- Edieresis.color1 

	- And 3012 more.

Use -F or --full-lists to disable shortening of long lists.
 [code: unreachable-glyphs]
</div></details><details><summary>⚠ <b>WARN:</b> Check if each glyph has the recommended amount of contours. (<a href="https://font-bakery.readthedocs.io/en/stable/fontbakery/profiles/universal.html#com.google.fonts/check/contour_count">com.google.fonts/check/contour_count</a>)</summary><div>


* ⚠ **WARN** This font has a 'Soft Hyphen' character (codepoint 0x00AD) which is supposed to be zero-width and invisible, and is used to mark a hyphenation possibility within a word in the absence of or overriding dictionary hyphenation. It is mostly an obsolete mechanism now, and the character is only included in fonts for legacy codepage coverage. [code: softhyphen]
* ⚠ **WARN** This check inspects the glyph outlines and detects the total number of contours in each of them. The expected values are infered from the typical ammounts of contours observed in a large collection of reference font families. The divergences listed below may simply indicate a significantly different design on some of your glyphs. On the other hand, some of these may flag actual bugs in the font such as glyphs mapped to an incorrect codepoint. Please consider reviewing the design and codepoint assignment of these to make sure they are correct.

The following glyphs do not have the recommended number of contours:

	- Glyph name: one	Contours detected: 2	Expected: 1

	- Glyph name: b	Contours detected: 1	Expected: 2

	- Glyph name: uni00AD	Contours detected: 1	Expected: 0

	- Glyph name: thorn	Contours detected: 3	Expected: 2

	- Glyph name: uni20A6	Contours detected: 2	Expected: 1, 3 or 5

	- Glyph name: uni20A9	Contours detected: 5	Expected: 1, 3, 4 or 7

	- Glyph name: b	Contours detected: 1	Expected: 2

	- Glyph name: one	Contours detected: 2	Expected: 1

	- Glyph name: thorn	Contours detected: 3	Expected: 2

	- Glyph name: uni00AD	Contours detected: 1	Expected: 0

	- Glyph name: uni20A6	Contours detected: 2	Expected: 1, 3 or 5 

	- And Glyph name: uni20A9	Contours detected: 5	Expected: 1, 3, 4 or 7
 [code: contour-count]
</div></details><details><summary>⚠ <b>WARN:</b> Ensure dotted circle glyph is present and can attach marks. (<a href="https://font-bakery.readthedocs.io/en/stable/fontbakery/profiles/universal.html#com.google.fonts/check/dotted_circle">com.google.fonts/check/dotted_circle</a>)</summary><div>


* ⚠ **WARN** No dotted circle glyph present [code: missing-dotted-circle]
</div></details><details><summary>⚠ <b>WARN:</b> Do outlines contain any jaggy segments? (<a href="https://font-bakery.readthedocs.io/en/stable/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_jaggy_segments">com.google.fonts/check/outline_jaggy_segments</a>)</summary><div>


* ⚠ **WARN** The following glyphs have jaggy segments:

	* q (U+0071): L<<517.0,-200.0>--<516.0,83.0>>/L<<516.0,83.0>--<516.0,0.0>> = 0.20245774221736668 [code: found-jaggy-segments]
</div></details><details><summary>⚠ <b>WARN:</b> Do outlines contain any semi-vertical or semi-horizontal lines? (<a href="https://font-bakery.readthedocs.io/en/stable/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_semi_vertical">com.google.fonts/check/outline_semi_vertical</a>)</summary><div>


* ⚠ **WARN** The following glyphs have semi-vertical/semi-horizontal lines:

	* T (U+0054): L<<277.0,0.0>--<278.0,519.0>>

	* Tcaron (U+0164): L<<277.0,0.0>--<278.0,519.0>>

	* ae (U+00E6): L<<1026.0,218.0>--<738.0,217.0>>

	* aeacute (U+01FD): L<<1026.0,218.0>--<738.0,217.0>>

	* ampersand (U+0026): L<<941.0,1.0>--<714.0,0.0>>

	* b (U+0062): L<<251.0,783.0>--<252.0,206.0>>

	* e (U+0065): L<<532.0,218.0>--<243.0,217.0>>

	* eacute (U+00E9): L<<532.0,218.0>--<243.0,217.0>>

	* ebreve (U+0115): L<<532.0,218.0>--<243.0,217.0>>

	* ecaron (U+011B): L<<532.0,218.0>--<243.0,217.0>> 

	* And 49 more.

Use -F or --full-lists to disable shortening of long lists. [code: found-semi-vertical]
</div></details><br></div></details><details><summary><b>[8] Foldit-Black.ttf</b></summary><div><details><summary>💔 <b>ERROR:</b> Check Google Fonts glyph coverage. (<a href="https://font-bakery.readthedocs.io/en/stable/fontbakery/profiles/googlefonts.html#com.google.fonts/check/glyph_coverage">com.google.fonts/check/glyph_coverage</a>)</summary><div>


* 💔 **ERROR** Failed with IndexError: list index out of range
</div></details><details><summary>⚠ <b>WARN:</b> Is there kerning info for non-ligated sequences? (<a href="https://font-bakery.readthedocs.io/en/stable/fontbakery/profiles/googlefonts.html#com.google.fonts/check/kerning_for_non_ligated_sequences">com.google.fonts/check/kerning_for_non_ligated_sequences</a>)</summary><div>


* ⚠ **WARN** GPOS table lacks kerning info for the following non-ligated sequences:

	- f + f

	- f + i

	- i + f

	- f + l

	- l + f 

	- And i + l [code: lacks-kern-info]
</div></details><details><summary>⚠ <b>WARN:</b> Ensure fonts have ScriptLangTags declared on the 'meta' table. (<a href="https://font-bakery.readthedocs.io/en/stable/fontbakery/profiles/googlefonts.html#com.google.fonts/check/meta/script_lang_tags">com.google.fonts/check/meta/script_lang_tags</a>)</summary><div>


* ⚠ **WARN** This font file does not have a 'meta' table. [code: lacks-meta-table]
</div></details><details><summary>⚠ <b>WARN:</b> Check font contains no unreachable glyphs (<a href="https://font-bakery.readthedocs.io/en/stable/fontbakery/profiles/universal.html#com.google.fonts/check/unreachable_glyphs">com.google.fonts/check/unreachable_glyphs</a>)</summary><div>


* ⚠ **WARN** The following glyphs could not be reached by codepoint or substitution rules:

	- ccaron.color0

	- ordfeminine.color0

	- colonmonetary.color4

	- registered.color7

	- Ccedilla.color0

	- uni020D.color1

	- uni1EE4.color0

	- uni032E.color0

	- ampersand.color4

	- Edieresis.color1 

	- And 3012 more.

Use -F or --full-lists to disable shortening of long lists.
 [code: unreachable-glyphs]
</div></details><details><summary>⚠ <b>WARN:</b> Check if each glyph has the recommended amount of contours. (<a href="https://font-bakery.readthedocs.io/en/stable/fontbakery/profiles/universal.html#com.google.fonts/check/contour_count">com.google.fonts/check/contour_count</a>)</summary><div>


* ⚠ **WARN** This font has a 'Soft Hyphen' character (codepoint 0x00AD) which is supposed to be zero-width and invisible, and is used to mark a hyphenation possibility within a word in the absence of or overriding dictionary hyphenation. It is mostly an obsolete mechanism now, and the character is only included in fonts for legacy codepage coverage. [code: softhyphen]
* ⚠ **WARN** This check inspects the glyph outlines and detects the total number of contours in each of them. The expected values are infered from the typical ammounts of contours observed in a large collection of reference font families. The divergences listed below may simply indicate a significantly different design on some of your glyphs. On the other hand, some of these may flag actual bugs in the font such as glyphs mapped to an incorrect codepoint. Please consider reviewing the design and codepoint assignment of these to make sure they are correct.

The following glyphs do not have the recommended number of contours:

	- Glyph name: one	Contours detected: 2	Expected: 1

	- Glyph name: b	Contours detected: 1	Expected: 2

	- Glyph name: uni00AD	Contours detected: 1	Expected: 0

	- Glyph name: thorn	Contours detected: 3	Expected: 2

	- Glyph name: uni20A6	Contours detected: 2	Expected: 1, 3 or 5

	- Glyph name: uni20A9	Contours detected: 5	Expected: 1, 3, 4 or 7

	- Glyph name: b	Contours detected: 1	Expected: 2

	- Glyph name: one	Contours detected: 2	Expected: 1

	- Glyph name: thorn	Contours detected: 3	Expected: 2

	- Glyph name: uni00AD	Contours detected: 1	Expected: 0

	- Glyph name: uni20A6	Contours detected: 2	Expected: 1, 3 or 5 

	- And Glyph name: uni20A9	Contours detected: 5	Expected: 1, 3, 4 or 7
 [code: contour-count]
</div></details><details><summary>⚠ <b>WARN:</b> Ensure dotted circle glyph is present and can attach marks. (<a href="https://font-bakery.readthedocs.io/en/stable/fontbakery/profiles/universal.html#com.google.fonts/check/dotted_circle">com.google.fonts/check/dotted_circle</a>)</summary><div>


* ⚠ **WARN** No dotted circle glyph present [code: missing-dotted-circle]
</div></details><details><summary>⚠ <b>WARN:</b> Do outlines contain any jaggy segments? (<a href="https://font-bakery.readthedocs.io/en/stable/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_jaggy_segments">com.google.fonts/check/outline_jaggy_segments</a>)</summary><div>


* ⚠ **WARN** The following glyphs have jaggy segments:

	* asterisk (U+002A): L<<225.0,442.0>--<211.0,351.0>>/L<<211.0,351.0>--<271.0,730.0>> = 0.24975216281029114

	* d (U+0064): L<<862.0,289.0>--<861.0,290.0>>/L<<861.0,290.0>--<863.0,287.0>> = 11.309932474020227

	* dcaron (U+010F): L<<862.0,289.0>--<861.0,290.0>>/L<<861.0,290.0>--<863.0,287.0>> = 11.309932474020227

	* dcroat (U+0111): L<<862.0,289.0>--<861.0,290.0>>/L<<861.0,290.0>--<863.0,287.0>> = 11.309932474020227

	* dong (U+20AB): L<<852.0,319.0>--<849.0,322.0>>/L<<849.0,322.0>--<853.0,317.0>> = 6.3401917459097925

	* oe (U+0153): L<<1201.0,221.0>--<842.0,220.0>>/L<<842.0,220.0>--<842.0,220.0>> = 0.15959785884710373

	* p (U+0070): L<<36.0,241.0>--<39.0,238.0>>/L<<39.0,238.0>--<35.0,243.0>> = 6.340191745909908 

	* And uni01C6 (U+01C6): L<<862.0,289.0>--<861.0,290.0>>/L<<861.0,290.0>--<863.0,287.0>> = 11.309932474020227 [code: found-jaggy-segments]
</div></details><details><summary>⚠ <b>WARN:</b> Do outlines contain any semi-vertical or semi-horizontal lines? (<a href="https://font-bakery.readthedocs.io/en/stable/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_semi_vertical">com.google.fonts/check/outline_semi_vertical</a>)</summary><div>


* ⚠ **WARN** The following glyphs have semi-vertical/semi-horizontal lines:

	* Euro (U+20AC): L<<344.0,333.0>--<824.0,334.0>>

	* Euro (U+20AC): L<<344.0,422.0>--<824.0,423.0>>

	* Euro (U+20AC): L<<847.0,310.0>--<344.0,309.0>>

	* Euro (U+20AC): L<<847.0,399.0>--<344.0,398.0>>

	* G (U+0047): L<<299.0,466.0>--<728.0,467.0>>

	* Gbreve (U+011E): L<<299.0,466.0>--<728.0,467.0>>

	* Gcaron (U+01E6): L<<299.0,466.0>--<728.0,467.0>>

	* Gcircumflex (U+011C): L<<299.0,466.0>--<728.0,467.0>>

	* Gdotaccent (U+0120): L<<299.0,466.0>--<728.0,467.0>>

	* T (U+0054): L<<305.0,0.0>--<306.0,486.0>> 

	* And 63 more.

Use -F or --full-lists to disable shortening of long lists. [code: found-semi-vertical]
</div></details><br></div></details><details><summary><b>[7] Foldit-Bold.ttf</b></summary><div><details><summary>💔 <b>ERROR:</b> Check Google Fonts glyph coverage. (<a href="https://font-bakery.readthedocs.io/en/stable/fontbakery/profiles/googlefonts.html#com.google.fonts/check/glyph_coverage">com.google.fonts/check/glyph_coverage</a>)</summary><div>


* 💔 **ERROR** Failed with IndexError: list index out of range
</div></details><details><summary>⚠ <b>WARN:</b> Is there kerning info for non-ligated sequences? (<a href="https://font-bakery.readthedocs.io/en/stable/fontbakery/profiles/googlefonts.html#com.google.fonts/check/kerning_for_non_ligated_sequences">com.google.fonts/check/kerning_for_non_ligated_sequences</a>)</summary><div>


* ⚠ **WARN** GPOS table lacks kerning info for the following non-ligated sequences:

	- f + f

	- f + i

	- i + f

	- f + l

	- l + f 

	- And i + l [code: lacks-kern-info]
</div></details><details><summary>⚠ <b>WARN:</b> Ensure fonts have ScriptLangTags declared on the 'meta' table. (<a href="https://font-bakery.readthedocs.io/en/stable/fontbakery/profiles/googlefonts.html#com.google.fonts/check/meta/script_lang_tags">com.google.fonts/check/meta/script_lang_tags</a>)</summary><div>


* ⚠ **WARN** This font file does not have a 'meta' table. [code: lacks-meta-table]
</div></details><details><summary>⚠ <b>WARN:</b> Check font contains no unreachable glyphs (<a href="https://font-bakery.readthedocs.io/en/stable/fontbakery/profiles/universal.html#com.google.fonts/check/unreachable_glyphs">com.google.fonts/check/unreachable_glyphs</a>)</summary><div>


* ⚠ **WARN** The following glyphs could not be reached by codepoint or substitution rules:

	- ccaron.color0

	- ordfeminine.color0

	- colonmonetary.color4

	- registered.color7

	- Ccedilla.color0

	- uni020D.color1

	- uni1EE4.color0

	- uni032E.color0

	- ampersand.color4

	- Edieresis.color1 

	- And 3012 more.

Use -F or --full-lists to disable shortening of long lists.
 [code: unreachable-glyphs]
</div></details><details><summary>⚠ <b>WARN:</b> Check if each glyph has the recommended amount of contours. (<a href="https://font-bakery.readthedocs.io/en/stable/fontbakery/profiles/universal.html#com.google.fonts/check/contour_count">com.google.fonts/check/contour_count</a>)</summary><div>


* ⚠ **WARN** This font has a 'Soft Hyphen' character (codepoint 0x00AD) which is supposed to be zero-width and invisible, and is used to mark a hyphenation possibility within a word in the absence of or overriding dictionary hyphenation. It is mostly an obsolete mechanism now, and the character is only included in fonts for legacy codepage coverage. [code: softhyphen]
* ⚠ **WARN** This check inspects the glyph outlines and detects the total number of contours in each of them. The expected values are infered from the typical ammounts of contours observed in a large collection of reference font families. The divergences listed below may simply indicate a significantly different design on some of your glyphs. On the other hand, some of these may flag actual bugs in the font such as glyphs mapped to an incorrect codepoint. Please consider reviewing the design and codepoint assignment of these to make sure they are correct.

The following glyphs do not have the recommended number of contours:

	- Glyph name: one	Contours detected: 2	Expected: 1

	- Glyph name: b	Contours detected: 1	Expected: 2

	- Glyph name: q	Contours detected: 1	Expected: 2

	- Glyph name: uni00AD	Contours detected: 1	Expected: 0

	- Glyph name: thorn	Contours detected: 3	Expected: 2

	- Glyph name: uni20A6	Contours detected: 4	Expected: 1, 3 or 5

	- Glyph name: uni20A9	Contours detected: 5	Expected: 1, 3, 4 or 7

	- Glyph name: b	Contours detected: 1	Expected: 2

	- Glyph name: one	Contours detected: 2	Expected: 1

	- Glyph name: q	Contours detected: 1	Expected: 2 

	- And 4 more.

Use -F or --full-lists to disable shortening of long lists.
 [code: contour-count]
</div></details><details><summary>⚠ <b>WARN:</b> Ensure dotted circle glyph is present and can attach marks. (<a href="https://font-bakery.readthedocs.io/en/stable/fontbakery/profiles/universal.html#com.google.fonts/check/dotted_circle">com.google.fonts/check/dotted_circle</a>)</summary><div>


* ⚠ **WARN** No dotted circle glyph present [code: missing-dotted-circle]
</div></details><details><summary>⚠ <b>WARN:</b> Do outlines contain any semi-vertical or semi-horizontal lines? (<a href="https://font-bakery.readthedocs.io/en/stable/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_semi_vertical">com.google.fonts/check/outline_semi_vertical</a>)</summary><div>


* ⚠ **WARN** The following glyphs have semi-vertical/semi-horizontal lines:

	* Euro (U+20AC): L<<263.0,341.0>--<605.0,342.0>>

	* Euro (U+20AC): L<<263.0,430.0>--<605.0,431.0>>

	* Euro (U+20AC): L<<628.0,318.0>--<263.0,317.0>>

	* Euro (U+20AC): L<<628.0,407.0>--<263.0,406.0>>

	* G (U+0047): L<<232.0,432.0>--<524.0,433.0>>

	* Gbreve (U+011E): L<<232.0,432.0>--<524.0,433.0>>

	* Gcaron (U+01E6): L<<232.0,432.0>--<524.0,433.0>>

	* Gcircumflex (U+011C): L<<232.0,432.0>--<524.0,433.0>>

	* Gdotaccent (U+0120): L<<232.0,432.0>--<524.0,433.0>>

	* M (U+004D): L<<42.0,722.0>--<188.0,723.0>> 

	* And 60 more.

Use -F or --full-lists to disable shortening of long lists. [code: found-semi-vertical]
</div></details><br></div></details><details><summary><b>[7] Foldit-Medium.ttf</b></summary><div><details><summary>💔 <b>ERROR:</b> Check Google Fonts glyph coverage. (<a href="https://font-bakery.readthedocs.io/en/stable/fontbakery/profiles/googlefonts.html#com.google.fonts/check/glyph_coverage">com.google.fonts/check/glyph_coverage</a>)</summary><div>


* 💔 **ERROR** Failed with IndexError: list index out of range
</div></details><details><summary>⚠ <b>WARN:</b> Is there kerning info for non-ligated sequences? (<a href="https://font-bakery.readthedocs.io/en/stable/fontbakery/profiles/googlefonts.html#com.google.fonts/check/kerning_for_non_ligated_sequences">com.google.fonts/check/kerning_for_non_ligated_sequences</a>)</summary><div>


* ⚠ **WARN** GPOS table lacks kerning info for the following non-ligated sequences:

	- f + f

	- f + i

	- i + f

	- f + l

	- l + f 

	- And i + l [code: lacks-kern-info]
</div></details><details><summary>⚠ <b>WARN:</b> Ensure fonts have ScriptLangTags declared on the 'meta' table. (<a href="https://font-bakery.readthedocs.io/en/stable/fontbakery/profiles/googlefonts.html#com.google.fonts/check/meta/script_lang_tags">com.google.fonts/check/meta/script_lang_tags</a>)</summary><div>


* ⚠ **WARN** This font file does not have a 'meta' table. [code: lacks-meta-table]
</div></details><details><summary>⚠ <b>WARN:</b> Check font contains no unreachable glyphs (<a href="https://font-bakery.readthedocs.io/en/stable/fontbakery/profiles/universal.html#com.google.fonts/check/unreachable_glyphs">com.google.fonts/check/unreachable_glyphs</a>)</summary><div>


* ⚠ **WARN** The following glyphs could not be reached by codepoint or substitution rules:

	- ccaron.color0

	- ordfeminine.color0

	- colonmonetary.color4

	- registered.color7

	- Ccedilla.color0

	- uni020D.color1

	- uni1EE4.color0

	- uni032E.color0

	- ampersand.color4

	- Edieresis.color1 

	- And 3012 more.

Use -F or --full-lists to disable shortening of long lists.
 [code: unreachable-glyphs]
</div></details><details><summary>⚠ <b>WARN:</b> Check if each glyph has the recommended amount of contours. (<a href="https://font-bakery.readthedocs.io/en/stable/fontbakery/profiles/universal.html#com.google.fonts/check/contour_count">com.google.fonts/check/contour_count</a>)</summary><div>


* ⚠ **WARN** This font has a 'Soft Hyphen' character (codepoint 0x00AD) which is supposed to be zero-width and invisible, and is used to mark a hyphenation possibility within a word in the absence of or overriding dictionary hyphenation. It is mostly an obsolete mechanism now, and the character is only included in fonts for legacy codepage coverage. [code: softhyphen]
* ⚠ **WARN** This check inspects the glyph outlines and detects the total number of contours in each of them. The expected values are infered from the typical ammounts of contours observed in a large collection of reference font families. The divergences listed below may simply indicate a significantly different design on some of your glyphs. On the other hand, some of these may flag actual bugs in the font such as glyphs mapped to an incorrect codepoint. Please consider reviewing the design and codepoint assignment of these to make sure they are correct.

The following glyphs do not have the recommended number of contours:

	- Glyph name: one	Contours detected: 2	Expected: 1

	- Glyph name: b	Contours detected: 1	Expected: 2

	- Glyph name: q	Contours detected: 1	Expected: 2

	- Glyph name: uni00AD	Contours detected: 1	Expected: 0

	- Glyph name: uni20A6	Contours detected: 4	Expected: 1, 3 or 5

	- Glyph name: uni20A9	Contours detected: 6	Expected: 1, 3, 4 or 7

	- Glyph name: b	Contours detected: 1	Expected: 2

	- Glyph name: one	Contours detected: 2	Expected: 1

	- Glyph name: q	Contours detected: 1	Expected: 2

	- Glyph name: uni00AD	Contours detected: 1	Expected: 0

	- Glyph name: uni20A6	Contours detected: 4	Expected: 1, 3 or 5 

	- And Glyph name: uni20A9	Contours detected: 6	Expected: 1, 3, 4 or 7
 [code: contour-count]
</div></details><details><summary>⚠ <b>WARN:</b> Ensure dotted circle glyph is present and can attach marks. (<a href="https://font-bakery.readthedocs.io/en/stable/fontbakery/profiles/universal.html#com.google.fonts/check/dotted_circle">com.google.fonts/check/dotted_circle</a>)</summary><div>


* ⚠ **WARN** No dotted circle glyph present [code: missing-dotted-circle]
</div></details><details><summary>⚠ <b>WARN:</b> Do outlines contain any semi-vertical or semi-horizontal lines? (<a href="https://font-bakery.readthedocs.io/en/stable/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_semi_vertical">com.google.fonts/check/outline_semi_vertical</a>)</summary><div>


* ⚠ **WARN** The following glyphs have semi-vertical/semi-horizontal lines:

	* Euro (U+20AC): L<<220.0,345.0>--<491.0,346.0>>

	* Euro (U+20AC): L<<220.0,434.0>--<491.0,435.0>>

	* Euro (U+20AC): L<<514.0,322.0>--<220.0,321.0>>

	* Euro (U+20AC): L<<514.0,411.0>--<220.0,410.0>>

	* G (U+0047): L<<196.0,414.0>--<418.0,415.0>>

	* Gbreve (U+011E): L<<196.0,414.0>--<418.0,415.0>>

	* Gcaron (U+01E6): L<<196.0,414.0>--<418.0,415.0>>

	* Gcircumflex (U+011C): L<<196.0,414.0>--<418.0,415.0>>

	* Gdotaccent (U+0120): L<<196.0,414.0>--<418.0,415.0>>

	* M (U+004D): L<<706.0,709.0>--<702.0,0.0>> 

	* And 44 more.

Use -F or --full-lists to disable shortening of long lists. [code: found-semi-vertical]
</div></details><br></div></details>
### Summary

| 💔 ERROR | 🔥 FAIL | ⚠ WARN | 💤 SKIP | ℹ INFO | 🍞 PASS | 🔎 DEBUG |
|:-----:|:----:|:----:|:----:|:----:|:----:|:----:|
| 9 | 0 | 61 | 1010 | 55 | 860 | 0 |
| 0% | 0% | 3% | 51% | 3% | 43% | 0% |

**Note:** The following loglevels were omitted in this report:
* **SKIP**
* **INFO**
* **PASS**
* **DEBUG**
