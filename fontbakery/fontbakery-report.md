## Fontbakery report

Fontbakery version: 0.8.2

<details>
<summary><b>[21] Foldit-[Expanded,ExtraBold].ttf</b></summary>
<details>
<summary>💔 <b>ERROR:</b> Check METADATA.pb includes production subsets.</summary>

* [com.google.fonts/check/metadata/includes_production_subsets](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/metadata/includes_production_subsets)
<pre>--- Rationale ---
Check METADATA.pb file includes the same subsets as the family in production.</pre>

* 💔 **ERROR** The condition <FontBakeryCondition:production_metadata> had an error: JSONDecodeError: Expecting value: line 1 column 1 (char 0)

</details>
<details>
<summary>💔 <b>ERROR:</b> Version number has increased since previous release on Google Fonts?</summary>

* [com.google.fonts/check/version_bump](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/version_bump)

* 💔 **ERROR** The condition <FontBakeryCondition:api_gfonts_ttFont> had an error: FailedConditionError: The condition <FontBakeryCondition:remote_styles> had an error: JSONDecodeError: Expecting value: line 1 column 1 (char 0)

</details>
<details>
<summary>💔 <b>ERROR:</b> Glyphs are similiar to Google Fonts version?</summary>

* [com.google.fonts/check/production_glyphs_similarity](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/production_glyphs_similarity)

* 💔 **ERROR** The condition <FontBakeryCondition:api_gfonts_ttFont> had an error: FailedConditionError: The condition <FontBakeryCondition:remote_styles> had an error: JSONDecodeError: Expecting value: line 1 column 1 (char 0)

</details>
<details>
<summary>💔 <b>ERROR:</b> Check if the vertical metrics of a family are similar to the same family hosted on Google Fonts.</summary>

* [com.google.fonts/check/vertical_metrics_regressions](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/vertical_metrics_regressions)
<pre>--- Rationale ---
If the family already exists on Google Fonts, we need to ensure that the checked
family&#x27;s vertical metrics are similar. This check will test the following schema
which was outlined in Fontbakery issue #1162 [1]:
- The family should visually have the same vertical metrics as the Regular style
hosted on Google Fonts.
- If the family on Google Fonts has differing hhea and typo metrics, the family
being checked should use the typo metrics for both the hhea and typo entries.
- If the family on Google Fonts has use typo metrics not enabled and the family
being checked has it enabled, the hhea and typo metrics should use the family on
Google Fonts winAscent and winDescent values.
- If the upms differ, the values must be scaled so the visual appearance is the
same.
[1] https://github.com/googlefonts/fontbakery/issues/1162</pre>

* 💔 **ERROR** The condition <FontBakeryCondition:regular_remote_style> had an error: FailedConditionError: The condition <FontBakeryCondition:remote_styles> had an error: JSONDecodeError: Expecting value: line 1 column 1 (char 0)

</details>
<details>
<summary>💔 <b>ERROR:</b> Check font follows the Google Fonts CJK vertical metric schema</summary>

* [com.google.fonts/check/cjk_vertical_metrics](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/cjk_vertical_metrics)
<pre>--- Rationale ---
CJK fonts have different vertical metrics when compared to Latin fonts. We
follow the schema developed by dr Ken Lunde for Source Han Sans and the Noto CJK
fonts.
Our documentation includes further information:
https://github.com/googlefonts/gf-docs/tree/main/Spec#cjk-vertical-metrics</pre>

* 💔 **ERROR** The condition <FontBakeryCondition:remote_styles> had an error: JSONDecodeError: Expecting value: line 1 column 1 (char 0)

</details>
<details>
<summary>💔 <b>ERROR:</b> Check if the vertical metrics of a CJK family are similar to the same family hosted on Google Fonts.</summary>

* [com.google.fonts/check/cjk_vertical_metrics_regressions](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/cjk_vertical_metrics_regressions)
<pre>--- Rationale ---
Check CJK family has the same vertical metrics as the same family hosted on
Google Fonts.</pre>

* 💔 **ERROR** The condition <FontBakeryCondition:regular_remote_style> had an error: FailedConditionError: The condition <FontBakeryCondition:remote_styles> had an error: JSONDecodeError: Expecting value: line 1 column 1 (char 0)

</details>
<details>
<summary>🔥 <b>FAIL:</b> Checking file is named canonically.</summary>

* [com.google.fonts/check/canonical_filename](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/canonical_filename)
<pre>--- Rationale ---
A font&#x27;s filename must be composed in the following manner:
&lt;familyname&gt;-&lt;stylename&gt;.ttf
- Nunito-Regular.ttf,
- Oswald-BoldItalic.ttf
Variable fonts must list the axis tags in alphabetical order in square brackets
and separated by commas:
- Roboto[wdth,wght].ttf
- Familyname-Italic[wght].ttf</pre>

* 🔥 **FAIL** Style name used in "fonts/ttf/Foldit-[Expanded,ExtraBold].ttf" is not canonical. You should rebuild the font using any of the following style names: "Thin", "ExtraLight", "Light", "Regular", "Medium", "SemiBold", "Bold", "ExtraBold", "Black", "Thin Italic", "ExtraLight Italic", "Light Italic", "Italic", "Medium Italic", "SemiBold Italic", "Bold Italic", "ExtraBold Italic", "Black Italic". [code: bad-static-filename]

</details>
<details>
<summary>🔥 <b>FAIL:</b> Check `Google Fonts Latin Core` glyph coverage.</summary>

* [com.google.fonts/check/glyph_coverage](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/glyph_coverage)
<pre>--- Rationale ---
Google Fonts expects that fonts in its collection support at least the minimal
set of characters defined in the `GF-latin-core` glyph-set.</pre>

* 🔥 **FAIL** Missing required codepoints: 0x00A0 (NO-BREAK SPACE) [code: missing-codepoints]

</details>
<details>
<summary>🔥 <b>FAIL:</b> Check copyright namerecords match license file.</summary>

* [com.google.fonts/check/name/license](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/name/license)
<pre>--- Rationale ---
A known licensing description must be provided in the NameID 14 (LICENSE
DESCRIPTION) entries of the name table.
The source of truth for this check (to determine which license is in use) is a
file placed side-by-side to your font project including the licensing terms.
Depending on the chosen license, one of the following string snippets is
expected to be found on the NameID 13 (LICENSE DESCRIPTION) entries of the name
table:
- &quot;This Font Software is licensed under the SIL Open Font License, Version 1.1.
This license is available with a FAQ at: https://scripts.sil.org/OFL&quot;
- &quot;Licensed under the Apache License, Version 2.0&quot;
- &quot;Licensed under the Ubuntu Font Licence 1.0.&quot;
Currently accepted licenses are Apache or Open Font License.
For a small set of legacy families the Ubuntu Font License may be acceptable as
well.
When in doubt, please choose OFL for new font projects.</pre>

* 🔥 **FAIL** License file OFL.txt exists but NameID 13 (LICENSE DESCRIPTION) value on platform 3 (WINDOWS) is not specified for that. Value was: "This Font Software is licensed under the SIL Open Font License, Version 1.1. This license..." Must be changed to "This Font Software is licensed under the SIL Open Font License, Version 1.1. This license is available with a FAQ at: https://scripts.sil.org/OFL" [code: wrong]

</details>
<details>
<summary>🔥 <b>FAIL:</b> Check name table: TYPOGRAPHIC_SUBFAMILY_NAME entries.</summary>

* [com.google.fonts/check/name/typographicsubfamilyname](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/name/typographicsubfamilyname)
<pre>--- Rationale ---
Requirements for the TYPOGRAPHIC_SUBFAMILY_NAME entries in the &#x27;name&#x27; table.</pre>

* 🔥 **FAIL** TYPOGRAPHIC_SUBFAMILY_NAME for Win "[Expanded,ExtraBold]" is incorrect. It must be "ExtraBold". [code: bad-typo-win]

</details>
<details>
<summary>🔥 <b>FAIL:</b> Checking OS/2 usWinAscent & usWinDescent.</summary>

* [com.google.fonts/check/family/win_ascent_and_descent](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/universal.html#com.google.fonts/check/family/win_ascent_and_descent)
<pre>--- Rationale ---
A font&#x27;s winAscent and winDescent values should be greater than the head table&#x27;s
yMax, abs(yMin) values. If they are less than these values, clipping can occur
on Windows platforms (https://github.com/RedHatBrand/Overpass/issues/33).
If the font includes tall/deep writing systems such as Arabic or Devanagari, the
winAscent and winDescent can be greater than the yMax and abs(yMin) to
accommodate vowel marks.
When the win Metrics are significantly greater than the upm, the linespacing can
appear too loose. To counteract this, enabling the OS/2 fsSelection bit 7
(Use_Typo_Metrics), will force Windows to use the OS/2 typo values instead. This
means the font developer can control the linespacing with the typo values,
whilst avoiding clipping by setting the win values to values greater than the
yMax and abs(yMin).</pre>

* 🔥 **FAIL** OS/2.usWinAscent value should be equal or greater than 1029, but got 800 instead [code: ascent]
* 🔥 **FAIL** OS/2.usWinDescent value should be equal or greater than 268, but got 200 instead. [code: descent]

</details>
<details>
<summary>🔥 <b>FAIL:</b> Font contains glyphs for whitespace characters?</summary>

* [com.google.fonts/check/whitespace_glyphs](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/universal.html#com.google.fonts/check/whitespace_glyphs)

* 🔥 **FAIL** Whitespace glyph missing for codepoint 0x00A0. [code: missing-whitespace-glyph-0x00A0]

</details>
<details>
<summary>⚠ <b>WARN:</b> Checking OS/2 achVendID.</summary>

* [com.google.fonts/check/vendor_id](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/vendor_id)
<pre>--- Rationale ---
Microsoft keeps a list of font vendors and their respective contact info. This
list is updated regularly and is indexed by a 4-char &quot;Vendor ID&quot; which is stored
in the achVendID field of the OS/2 table.
Registering your ID is not mandatory, but it is a good practice since some
applications may display the type designer / type foundry contact info on some
dialog and also because that info will be visible on Microsoft&#x27;s website:
https://docs.microsoft.com/en-us/typography/vendors/
This check verifies whether or not a given font&#x27;s vendor ID is registered in
that list or if it has some of the default values used by the most common font
editors.
Each new FontBakery release includes a cached copy of that list of vendor IDs.
If you registered recently, you&#x27;re safe to ignore warnings emitted by this
check, since your ID will soon be included in one of our upcoming releases.</pre>

* ⚠ **WARN** OS/2 VendorID value 'NONE' is not yet recognized. If you registered it recently, then it's safe to ignore this warning message. Otherwise, you should set it to your own unique 4 character code, and register it with Microsoft at https://www.microsoft.com/typography/links/vendorlist.aspx
 [code: unknown]

</details>
<details>
<summary>⚠ <b>WARN:</b> Font has old ttfautohint applied?</summary>

* [com.google.fonts/check/old_ttfautohint](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/old_ttfautohint)
<pre>--- Rationale ---
Check if font has been hinted with an outdated version of ttfautohint.</pre>

* ⚠ **WARN** ttfautohint used in font = 1.8.3; latest = 1.8.4; Need to re-run with the newer version! [code: old-ttfa]

</details>
<details>
<summary>⚠ <b>WARN:</b> Check if each glyph has the recommended amount of contours.</summary>

* [com.google.fonts/check/contour_count](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/contour_count)
<pre>--- Rationale ---
Visually QAing thousands of glyphs by hand is tiring. Most glyphs can only be
constructured in a handful of ways. This means a glyph&#x27;s contour count will only
differ slightly amongst different fonts, e.g a &#x27;g&#x27; could either be 2 or 3
contours, depending on whether its double story or single story.
However, a quotedbl should have 2 contours, unless the font belongs to a display
family.
This check currently does not cover variable fonts because there&#x27;s plenty of
alternative ways of constructing glyphs with multiple outlines for each feature
in a VarFont. The expected contour count data for this check is currently
optimized for the typical construction of glyphs in static fonts.</pre>

* ⚠ **WARN** This check inspects the glyph outlines and detects the total number of contours in each of them. The expected values are infered from the typical ammounts of contours observed in a large collection of reference font families. The divergences listed below may simply indicate a significantly different design on some of your glyphs. On the other hand, some of these may flag actual bugs in the font such as glyphs mapped to an incorrect codepoint. Please consider reviewing the design and codepoint assignment of these to make sure they are correct.

The following glyphs do not have the recommended number of contours:

Glyph name: one	Contours detected: 2	Expected: 1
Glyph name: at	Contours detected: 1	Expected: 2
Glyph name: I	Contours detected: 2	Expected: 1
Glyph name: y	Contours detected: 2	Expected: 1
Glyph name: uni00B9	Contours detected: 2	Expected: 1
Glyph name: onehalf	Contours detected: 4	Expected: 3
Glyph name: Igrave	Contours detected: 3	Expected: 2
Glyph name: Iacute	Contours detected: 3	Expected: 2
Glyph name: Icircumflex	Contours detected: 3	Expected: 2
Glyph name: Idieresis	Contours detected: 4	Expected: 3
Glyph name: Eth	Contours detected: 3	Expected: 2
Glyph name: eth	Contours detected: 3	Expected: 2
Glyph name: yacute	Contours detected: 3	Expected: 2
Glyph name: thorn	Contours detected: 1	Expected: 2
Glyph name: ydieresis	Contours detected: 4	Expected: 3
Glyph name: aogonek	Contours detected: 3	Expected: 2
Glyph name: Dcroat	Contours detected: 3	Expected: 2
Glyph name: dcroat	Contours detected: 3	Expected: 2
Glyph name: eogonek	Contours detected: 3	Expected: 2
Glyph name: Itilde	Contours detected: 3	Expected: 2
Glyph name: Imacron	Contours detected: 3	Expected: 2
Glyph name: Ibreve	Contours detected: 3	Expected: 2
Glyph name: Iogonek	Contours detected: 3	Expected: 1 or 2
Glyph name: Idotaccent	Contours detected: 3	Expected: 2
Glyph name: Tbar	Contours detected: 2	Expected: 1
Glyph name: Uogonek	Contours detected: 2	Expected: 1
Glyph name: uogonek	Contours detected: 2	Expected: 1
Glyph name: ycircumflex	Contours detected: 3	Expected: 2
Glyph name: ohorn	Contours detected: 3	Expected: 2
Glyph name: Uhorn	Contours detected: 2	Expected: 1
Glyph name: uhorn	Contours detected: 2	Expected: 1
Glyph name: uni01EA	Contours detected: 3	Expected: 2
Glyph name: uni01EB	Contours detected: 3	Expected: 2
Glyph name: uni0203	Contours detected: 4	Expected: 3
Glyph name: uni0207	Contours detected: 4	Expected: 3
Glyph name: uni0208	Contours detected: 4	Expected: 3
Glyph name: uni020A	Contours detected: 3	Expected: 2
Glyph name: uni020F	Contours detected: 4	Expected: 3
Glyph name: uni0213	Contours detected: 3	Expected: 2
Glyph name: uni0217	Contours detected: 3	Expected: 2
Glyph name: uni0233	Contours detected: 3	Expected: 2
Glyph name: uni0311	Contours detected: 2	Expected: 1
Glyph name: uni1EC8	Contours detected: 3	Expected: 2
Glyph name: uni1ECA	Contours detected: 3	Expected: 2
Glyph name: uni1EDB	Contours detected: 4	Expected: 3
Glyph name: uni1EDD	Contours detected: 4	Expected: 3
Glyph name: uni1EDF	Contours detected: 4	Expected: 3
Glyph name: uni1EE1	Contours detected: 4	Expected: 3
Glyph name: uni1EE3	Contours detected: 4	Expected: 3
Glyph name: uni1EE8	Contours detected: 3	Expected: 2
Glyph name: uni1EE9	Contours detected: 3	Expected: 2
Glyph name: uni1EEA	Contours detected: 3	Expected: 2
Glyph name: uni1EEB	Contours detected: 3	Expected: 2
Glyph name: uni1EEC	Contours detected: 3	Expected: 2
Glyph name: uni1EED	Contours detected: 3	Expected: 2
Glyph name: uni1EEE	Contours detected: 3	Expected: 2
Glyph name: uni1EEF	Contours detected: 3	Expected: 2
Glyph name: uni1EF0	Contours detected: 3	Expected: 2
Glyph name: uni1EF1	Contours detected: 3	Expected: 2
Glyph name: ygrave	Contours detected: 3	Expected: 2
Glyph name: uni1EF5	Contours detected: 3	Expected: 2
Glyph name: uni1EF7	Contours detected: 3	Expected: 2
Glyph name: uni1EF9	Contours detected: 3	Expected: 2
Glyph name: uni20A6	Contours detected: 2	Expected: 1, 3 or 5
Glyph name: uni20A9	Contours detected: 5	Expected: 1, 3, 4 or 7
Glyph name: uni20BA	Contours detected: 2	Expected: 1
Glyph name: Dcroat	Contours detected: 3	Expected: 2
Glyph name: Eth	Contours detected: 3	Expected: 2
Glyph name: I	Contours detected: 2	Expected: 1
Glyph name: Iacute	Contours detected: 3	Expected: 2
Glyph name: Ibreve	Contours detected: 3	Expected: 2
Glyph name: Icircumflex	Contours detected: 3	Expected: 2
Glyph name: Idieresis	Contours detected: 4	Expected: 3
Glyph name: Idotaccent	Contours detected: 3	Expected: 2
Glyph name: Igrave	Contours detected: 3	Expected: 2
Glyph name: Imacron	Contours detected: 3	Expected: 2
Glyph name: Iogonek	Contours detected: 3	Expected: 1 or 2
Glyph name: Itilde	Contours detected: 3	Expected: 2
Glyph name: Tbar	Contours detected: 2	Expected: 1
Glyph name: Uhorn	Contours detected: 2	Expected: 1
Glyph name: Uogonek	Contours detected: 2	Expected: 1
Glyph name: aogonek	Contours detected: 3	Expected: 2
Glyph name: at	Contours detected: 1	Expected: 2
Glyph name: dcroat	Contours detected: 3	Expected: 2
Glyph name: eogonek	Contours detected: 3	Expected: 2
Glyph name: eth	Contours detected: 3	Expected: 2
Glyph name: ohorn	Contours detected: 3	Expected: 2
Glyph name: one	Contours detected: 2	Expected: 1
Glyph name: onehalf	Contours detected: 4	Expected: 3
Glyph name: thorn	Contours detected: 1	Expected: 2
Glyph name: uhorn	Contours detected: 2	Expected: 1
Glyph name: uni0233	Contours detected: 3	Expected: 2
Glyph name: uni0311	Contours detected: 2	Expected: 1
Glyph name: uni1EC8	Contours detected: 3	Expected: 2
Glyph name: uni1ECA	Contours detected: 3	Expected: 2
Glyph name: uni1EDB	Contours detected: 4	Expected: 3
Glyph name: uni1EDD	Contours detected: 4	Expected: 3
Glyph name: uni1EDF	Contours detected: 4	Expected: 3
Glyph name: uni1EE1	Contours detected: 4	Expected: 3
Glyph name: uni1EE3	Contours detected: 4	Expected: 3
Glyph name: uni1EE8	Contours detected: 3	Expected: 2
Glyph name: uni1EE9	Contours detected: 3	Expected: 2
Glyph name: uni1EEA	Contours detected: 3	Expected: 2
Glyph name: uni1EEB	Contours detected: 3	Expected: 2
Glyph name: uni1EEC	Contours detected: 3	Expected: 2
Glyph name: uni1EED	Contours detected: 3	Expected: 2
Glyph name: uni1EEE	Contours detected: 3	Expected: 2
Glyph name: uni1EEF	Contours detected: 3	Expected: 2
Glyph name: uni1EF0	Contours detected: 3	Expected: 2
Glyph name: uni1EF1	Contours detected: 3	Expected: 2
Glyph name: uni1EF5	Contours detected: 3	Expected: 2
Glyph name: uni1EF7	Contours detected: 3	Expected: 2
Glyph name: uni1EF9	Contours detected: 3	Expected: 2
Glyph name: uni20A6	Contours detected: 2	Expected: 1, 3 or 5
Glyph name: uni20A9	Contours detected: 5	Expected: 1, 3, 4 or 7
Glyph name: uni20BA	Contours detected: 2	Expected: 1
Glyph name: uogonek	Contours detected: 2	Expected: 1
Glyph name: y	Contours detected: 2	Expected: 1
Glyph name: yacute	Contours detected: 3	Expected: 2
Glyph name: ycircumflex	Contours detected: 3	Expected: 2
Glyph name: ydieresis	Contours detected: 4	Expected: 3
Glyph name: ygrave	Contours detected: 3	Expected: 2 [code: contour-count]

</details>
<details>
<summary>⚠ <b>WARN:</b> Are there caret positions declared for every ligature?</summary>

* [com.google.fonts/check/ligature_carets](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/ligature_carets)
<pre>--- Rationale ---
All ligatures in a font must have corresponding caret (text cursor) positions
defined in the GDEF table, otherwhise, users may experience issues with caret
rendering.
If using GlyphsApp or UFOs, ligature carets can be defined as anchors with names
starting with &#x27;caret_&#x27;. These can be compiled with fontmake as of version
v2.4.0.</pre>

* ⚠ **WARN** This font lacks caret position values for ligature glyphs on its GDEF table. [code: lacks-caret-pos]

</details>
<details>
<summary>⚠ <b>WARN:</b> Is there kerning info for non-ligated sequences?</summary>

* [com.google.fonts/check/kerning_for_non_ligated_sequences](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/kerning_for_non_ligated_sequences)
<pre>--- Rationale ---
Fonts with ligatures should have kerning on the corresponding non-ligated
sequences for text where ligatures aren&#x27;t used (eg
https://github.com/impallari/Raleway/issues/14).</pre>

* ⚠ **WARN** GPOS table lacks kerning info for the following non-ligated sequences:
	- f + f
	- f + i
	- i + f
	- f + l
	- l + f
	- i + l

   [code: lacks-kern-info]

</details>
<details>
<summary>⚠ <b>WARN:</b> Combined length of family and style must not exceed 27 characters.</summary>

* [com.google.fonts/check/name/family_and_style_max_length](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/name/family_and_style_max_length)
<pre>--- Rationale ---
According to a GlyphsApp tutorial [1], in order to make sure all versions of
Windows recognize it as a valid font file, we must make sure that the
concatenated length of the familyname (NameID.FONT_FAMILY_NAME) and style
(NameID.FONT_SUBFAMILY_NAME) strings in the name table do not exceed 20
characters.
After discussing the problem in more detail at `FontBakery issue #2179 [2] we
decided that allowing up to 27 chars would still be on the safe side, though.
[1] https://glyphsapp.com/tutorials/multiple-masters-part-3-setting-up-instances
[2] https://github.com/googlefonts/fontbakery/issues/2179</pre>

* ⚠ **WARN** The combined length of family and style exceeds 27 chars in the following 'WINDOWS' entries:
 FONT_FAMILY_NAME = 'Foldit [Expanded,ExtraBold]' / SUBFAMILY_NAME = 'Regular'

Please take a look at the conversation at https://github.com/googlefonts/fontbakery/issues/2179 in order to understand the reasoning behind these name table records max-length criteria. [code: too-long]

</details>
<details>
<summary>⚠ <b>WARN:</b> Ensure fonts have ScriptLangTags declared on the 'meta' table.</summary>

* [com.google.fonts/check/meta/script_lang_tags](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/meta/script_lang_tags)
<pre>--- Rationale ---
The OpenType &#x27;meta&#x27; table originated at Apple. Microsoft added it to OT with
just two DataMap records:
- dlng: comma-separated ScriptLangTags that indicate which scripts, or languages
and scripts, with possible variants, the font is designed for
- slng: comma-separated ScriptLangTags that indicate which scripts, or languages
and scripts, with possible variants, the font supports
The slng structure is intended to describe which languages and scripts the font
overall supports. For example, a Traditional Chinese font that also contains
Latin characters, can indicate Hant,Latn, showing that it supports Hant, the
Traditional Chinese variant of the Hani script, and it also supports the Latn
script
The dlng structure is far more interesting. A font may contain various glyphs,
but only a particular subset of the glyphs may be truly &quot;leading&quot; in the design,
while other glyphs may have been included for technical reasons. Such a
Traditional Chinese font could only list Hant there, showing that it’s designed
for Traditional Chinese, but the font would omit Latn, because the developers
don’t think the font is really recommended for purely Latin-script use.
The tags used in the structures can comprise just script, or also language and
script. For example, if a font has Bulgarian Cyrillic alternates in the locl
feature for the cyrl BGR OT languagesystem, it could also indicate in dlng
explicitly that it supports bul-Cyrl. (Note that the scripts and languages in
meta use the ISO language and script codes, not the OpenType ones).
This check ensures that the font has the meta table containing the slng and dlng
structures.
All families in the Google Fonts collection should contain the &#x27;meta&#x27; table.
Windows 10 already uses it when deciding on which fonts to fall back to. The
Google Fonts API and also other environments could use the data for smarter
filtering. Most importantly, those entries should be added to the Noto fonts.
In the font making process, some environments store this data in external files
already. But the meta table provides a convenient way to store this inside the
font file, so some tools may add the data, and unrelated tools may read this
data. This makes the solution much more portable and universal.</pre>

* ⚠ **WARN** This font file does not have a 'meta' table. [code: lacks-meta-table]

</details>
<details>
<summary>⚠ <b>WARN:</b> Do outlines contain any jaggy segments?</summary>

* [com.google.fonts/check/outline_jaggy_segments](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_jaggy_segments)
<pre>--- Rationale ---
This check heuristically detects outline segments which form a particularly
small angle, indicative of an outline error. This may cause false positives in
cases such as extreme ink traps, so should be regarded as advisory and backed up
by manual inspection.</pre>

* ⚠ **WARN** The following glyphs have jaggy segments:
	* asterisk (U+002A): L<<265.0,442.0>--<251.0,351.0>>/L<<251.0,351.0>--<311.0,730.0>> = 0.24975216281029114
	* d (U+0064): L<<782.0,329.0>--<780.0,331.0>>/L<<780.0,331.0>--<783.0,327.0>> = 8.13010235415596
	* dcaron (U+010F): L<<782.0,329.0>--<780.0,331.0>>/L<<780.0,331.0>--<783.0,327.0>> = 8.13010235415596
	* dcroat (U+0111): L<<782.0,329.0>--<780.0,331.0>>/L<<780.0,331.0>--<783.0,327.0>> = 8.13010235415596
	* dong (U+20AB): L<<782.0,377.0>--<780.0,379.0>>/L<<780.0,379.0>--<783.0,375.0>> = 8.13010235415596
	* eth (U+00F0): L<<782.0,329.0>--<781.0,330.0>>/L<<781.0,330.0>--<783.0,327.0>> = 11.309932474020227
	* kgreenlandic (U+0138): L<<248.0,794.0>--<249.0,400.0>>/L<<249.0,400.0>--<249.0,437.0>> = 0.1454204479278869
	* p (U+0070): L<<36.0,201.0>--<38.0,199.0>>/L<<38.0,199.0>--<35.0,203.0>> = 8.13010235415596
	* thorn (U+00FE): L<<36.0,201.0>--<38.0,199.0>>/L<<38.0,199.0>--<35.0,203.0>> = 8.13010235415596
	* uni01C6 (U+01C6): L<<782.0,329.0>--<780.0,331.0>>/L<<780.0,331.0>--<783.0,327.0>> = 8.13010235415596
	* uni20BA (U+20BA): L<<-109.0,455.0>--<-112.0,425.0>>/L<<-112.0,425.0>--<-112.0,576.0>> = 5.710593137499633 and uni20BA (U+20BA): L<<593.0,565.0>--<593.0,496.0>>/L<<593.0,496.0>--<592.0,565.0>> = 0.8303154862578446 [code: found-jaggy-segments]

</details>
<details>
<summary>⚠ <b>WARN:</b> Do outlines contain any semi-vertical or semi-horizontal lines?</summary>

* [com.google.fonts/check/outline_semi_vertical](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_semi_vertical)
<pre>--- Rationale ---
This check detects line segments which are nearly, but not quite, exactly
horizontal or vertical. Sometimes such lines are created by design, but often
they are indicative of a design error.
This check is disabled for italic styles, which often contain nearly-upright
lines.</pre>

* ⚠ **WARN** The following glyphs have semi-vertical/semi-horizontal lines:
 * Euro (U+20AC): L<<344.0,333.0>--<824.0,334.0>>
 * Euro (U+20AC): L<<344.0,422.0>--<824.0,423.0>>
 * Euro (U+20AC): L<<847.0,310.0>--<344.0,309.0>>
 * Euro (U+20AC): L<<847.0,399.0>--<344.0,398.0>>
 * I (U+0049): L<<245.0,0.0>--<246.0,486.0>>
 * I (U+0049): L<<245.0,0.0>--<25.0,1.0>>
 * Iacute (U+00CD): L<<245.0,0.0>--<246.0,486.0>>
 * Iacute (U+00CD): L<<245.0,0.0>--<25.0,1.0>>
 * Ibreve (U+012C): L<<245.0,0.0>--<246.0,486.0>>
 * Ibreve (U+012C): L<<245.0,0.0>--<25.0,1.0>> and 91 more. [code: found-semi-vertical]

</details>
<br>
</details>
<details>
<summary><b>[22] Foldit-[Condensed,Thin].ttf</b></summary>
<details>
<summary>💔 <b>ERROR:</b> Check METADATA.pb includes production subsets.</summary>

* [com.google.fonts/check/metadata/includes_production_subsets](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/metadata/includes_production_subsets)
<pre>--- Rationale ---
Check METADATA.pb file includes the same subsets as the family in production.</pre>

* 💔 **ERROR** The condition <FontBakeryCondition:production_metadata> had an error: JSONDecodeError: Expecting value: line 1 column 1 (char 0)

</details>
<details>
<summary>💔 <b>ERROR:</b> Version number has increased since previous release on Google Fonts?</summary>

* [com.google.fonts/check/version_bump](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/version_bump)

* 💔 **ERROR** The condition <FontBakeryCondition:api_gfonts_ttFont> had an error: FailedConditionError: The condition <FontBakeryCondition:remote_styles> had an error: JSONDecodeError: Expecting value: line 1 column 1 (char 0)

</details>
<details>
<summary>💔 <b>ERROR:</b> Glyphs are similiar to Google Fonts version?</summary>

* [com.google.fonts/check/production_glyphs_similarity](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/production_glyphs_similarity)

* 💔 **ERROR** The condition <FontBakeryCondition:api_gfonts_ttFont> had an error: FailedConditionError: The condition <FontBakeryCondition:remote_styles> had an error: JSONDecodeError: Expecting value: line 1 column 1 (char 0)

</details>
<details>
<summary>💔 <b>ERROR:</b> Check if the vertical metrics of a family are similar to the same family hosted on Google Fonts.</summary>

* [com.google.fonts/check/vertical_metrics_regressions](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/vertical_metrics_regressions)
<pre>--- Rationale ---
If the family already exists on Google Fonts, we need to ensure that the checked
family&#x27;s vertical metrics are similar. This check will test the following schema
which was outlined in Fontbakery issue #1162 [1]:
- The family should visually have the same vertical metrics as the Regular style
hosted on Google Fonts.
- If the family on Google Fonts has differing hhea and typo metrics, the family
being checked should use the typo metrics for both the hhea and typo entries.
- If the family on Google Fonts has use typo metrics not enabled and the family
being checked has it enabled, the hhea and typo metrics should use the family on
Google Fonts winAscent and winDescent values.
- If the upms differ, the values must be scaled so the visual appearance is the
same.
[1] https://github.com/googlefonts/fontbakery/issues/1162</pre>

* 💔 **ERROR** The condition <FontBakeryCondition:regular_remote_style> had an error: FailedConditionError: The condition <FontBakeryCondition:remote_styles> had an error: JSONDecodeError: Expecting value: line 1 column 1 (char 0)

</details>
<details>
<summary>💔 <b>ERROR:</b> Check font follows the Google Fonts CJK vertical metric schema</summary>

* [com.google.fonts/check/cjk_vertical_metrics](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/cjk_vertical_metrics)
<pre>--- Rationale ---
CJK fonts have different vertical metrics when compared to Latin fonts. We
follow the schema developed by dr Ken Lunde for Source Han Sans and the Noto CJK
fonts.
Our documentation includes further information:
https://github.com/googlefonts/gf-docs/tree/main/Spec#cjk-vertical-metrics</pre>

* 💔 **ERROR** The condition <FontBakeryCondition:remote_styles> had an error: JSONDecodeError: Expecting value: line 1 column 1 (char 0)

</details>
<details>
<summary>💔 <b>ERROR:</b> Check if the vertical metrics of a CJK family are similar to the same family hosted on Google Fonts.</summary>

* [com.google.fonts/check/cjk_vertical_metrics_regressions](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/cjk_vertical_metrics_regressions)
<pre>--- Rationale ---
Check CJK family has the same vertical metrics as the same family hosted on
Google Fonts.</pre>

* 💔 **ERROR** The condition <FontBakeryCondition:regular_remote_style> had an error: FailedConditionError: The condition <FontBakeryCondition:remote_styles> had an error: JSONDecodeError: Expecting value: line 1 column 1 (char 0)

</details>
<details>
<summary>🔥 <b>FAIL:</b> Checking file is named canonically.</summary>

* [com.google.fonts/check/canonical_filename](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/canonical_filename)
<pre>--- Rationale ---
A font&#x27;s filename must be composed in the following manner:
&lt;familyname&gt;-&lt;stylename&gt;.ttf
- Nunito-Regular.ttf,
- Oswald-BoldItalic.ttf
Variable fonts must list the axis tags in alphabetical order in square brackets
and separated by commas:
- Roboto[wdth,wght].ttf
- Familyname-Italic[wght].ttf</pre>

* 🔥 **FAIL** Style name used in "fonts/ttf/Foldit-[Condensed,Thin].ttf" is not canonical. You should rebuild the font using any of the following style names: "Thin", "ExtraLight", "Light", "Regular", "Medium", "SemiBold", "Bold", "ExtraBold", "Black", "Thin Italic", "ExtraLight Italic", "Light Italic", "Italic", "Medium Italic", "SemiBold Italic", "Bold Italic", "ExtraBold Italic", "Black Italic". [code: bad-static-filename]

</details>
<details>
<summary>🔥 <b>FAIL:</b> Check `Google Fonts Latin Core` glyph coverage.</summary>

* [com.google.fonts/check/glyph_coverage](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/glyph_coverage)
<pre>--- Rationale ---
Google Fonts expects that fonts in its collection support at least the minimal
set of characters defined in the `GF-latin-core` glyph-set.</pre>

* 🔥 **FAIL** Missing required codepoints: 0x00A0 (NO-BREAK SPACE) [code: missing-codepoints]

</details>
<details>
<summary>🔥 <b>FAIL:</b> Check copyright namerecords match license file.</summary>

* [com.google.fonts/check/name/license](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/name/license)
<pre>--- Rationale ---
A known licensing description must be provided in the NameID 14 (LICENSE
DESCRIPTION) entries of the name table.
The source of truth for this check (to determine which license is in use) is a
file placed side-by-side to your font project including the licensing terms.
Depending on the chosen license, one of the following string snippets is
expected to be found on the NameID 13 (LICENSE DESCRIPTION) entries of the name
table:
- &quot;This Font Software is licensed under the SIL Open Font License, Version 1.1.
This license is available with a FAQ at: https://scripts.sil.org/OFL&quot;
- &quot;Licensed under the Apache License, Version 2.0&quot;
- &quot;Licensed under the Ubuntu Font Licence 1.0.&quot;
Currently accepted licenses are Apache or Open Font License.
For a small set of legacy families the Ubuntu Font License may be acceptable as
well.
When in doubt, please choose OFL for new font projects.</pre>

* 🔥 **FAIL** License file OFL.txt exists but NameID 13 (LICENSE DESCRIPTION) value on platform 3 (WINDOWS) is not specified for that. Value was: "This Font Software is licensed under the SIL Open Font License, Version 1.1. This license..." Must be changed to "This Font Software is licensed under the SIL Open Font License, Version 1.1. This license is available with a FAQ at: https://scripts.sil.org/OFL" [code: wrong]

</details>
<details>
<summary>🔥 <b>FAIL:</b> Check name table: TYPOGRAPHIC_SUBFAMILY_NAME entries.</summary>

* [com.google.fonts/check/name/typographicsubfamilyname](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/name/typographicsubfamilyname)
<pre>--- Rationale ---
Requirements for the TYPOGRAPHIC_SUBFAMILY_NAME entries in the &#x27;name&#x27; table.</pre>

* 🔥 **FAIL** TYPOGRAPHIC_SUBFAMILY_NAME for Win "[Condensed,Thin]" is incorrect. It must be "Thin". [code: bad-typo-win]

</details>
<details>
<summary>🔥 <b>FAIL:</b> Checking OS/2 usWinAscent & usWinDescent.</summary>

* [com.google.fonts/check/family/win_ascent_and_descent](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/universal.html#com.google.fonts/check/family/win_ascent_and_descent)
<pre>--- Rationale ---
A font&#x27;s winAscent and winDescent values should be greater than the head table&#x27;s
yMax, abs(yMin) values. If they are less than these values, clipping can occur
on Windows platforms (https://github.com/RedHatBrand/Overpass/issues/33).
If the font includes tall/deep writing systems such as Arabic or Devanagari, the
winAscent and winDescent can be greater than the yMax and abs(yMin) to
accommodate vowel marks.
When the win Metrics are significantly greater than the upm, the linespacing can
appear too loose. To counteract this, enabling the OS/2 fsSelection bit 7
(Use_Typo_Metrics), will force Windows to use the OS/2 typo values instead. This
means the font developer can control the linespacing with the typo values,
whilst avoiding clipping by setting the win values to values greater than the
yMax and abs(yMin).</pre>

* 🔥 **FAIL** OS/2.usWinAscent value should be equal or greater than 1029, but got 800 instead [code: ascent]
* 🔥 **FAIL** OS/2.usWinDescent value should be equal or greater than 268, but got 200 instead. [code: descent]

</details>
<details>
<summary>🔥 <b>FAIL:</b> Font contains glyphs for whitespace characters?</summary>

* [com.google.fonts/check/whitespace_glyphs](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/universal.html#com.google.fonts/check/whitespace_glyphs)

* 🔥 **FAIL** Whitespace glyph missing for codepoint 0x00A0. [code: missing-whitespace-glyph-0x00A0]

</details>
<details>
<summary>⚠ <b>WARN:</b> Checking OS/2 achVendID.</summary>

* [com.google.fonts/check/vendor_id](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/vendor_id)
<pre>--- Rationale ---
Microsoft keeps a list of font vendors and their respective contact info. This
list is updated regularly and is indexed by a 4-char &quot;Vendor ID&quot; which is stored
in the achVendID field of the OS/2 table.
Registering your ID is not mandatory, but it is a good practice since some
applications may display the type designer / type foundry contact info on some
dialog and also because that info will be visible on Microsoft&#x27;s website:
https://docs.microsoft.com/en-us/typography/vendors/
This check verifies whether or not a given font&#x27;s vendor ID is registered in
that list or if it has some of the default values used by the most common font
editors.
Each new FontBakery release includes a cached copy of that list of vendor IDs.
If you registered recently, you&#x27;re safe to ignore warnings emitted by this
check, since your ID will soon be included in one of our upcoming releases.</pre>

* ⚠ **WARN** OS/2 VendorID value 'NONE' is not yet recognized. If you registered it recently, then it's safe to ignore this warning message. Otherwise, you should set it to your own unique 4 character code, and register it with Microsoft at https://www.microsoft.com/typography/links/vendorlist.aspx
 [code: unknown]

</details>
<details>
<summary>⚠ <b>WARN:</b> Font has old ttfautohint applied?</summary>

* [com.google.fonts/check/old_ttfautohint](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/old_ttfautohint)
<pre>--- Rationale ---
Check if font has been hinted with an outdated version of ttfautohint.</pre>

* ⚠ **WARN** ttfautohint used in font = 1.8.3; latest = 1.8.4; Need to re-run with the newer version! [code: old-ttfa]

</details>
<details>
<summary>⚠ <b>WARN:</b> Check if each glyph has the recommended amount of contours.</summary>

* [com.google.fonts/check/contour_count](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/contour_count)
<pre>--- Rationale ---
Visually QAing thousands of glyphs by hand is tiring. Most glyphs can only be
constructured in a handful of ways. This means a glyph&#x27;s contour count will only
differ slightly amongst different fonts, e.g a &#x27;g&#x27; could either be 2 or 3
contours, depending on whether its double story or single story.
However, a quotedbl should have 2 contours, unless the font belongs to a display
family.
This check currently does not cover variable fonts because there&#x27;s plenty of
alternative ways of constructing glyphs with multiple outlines for each feature
in a VarFont. The expected contour count data for this check is currently
optimized for the typical construction of glyphs in static fonts.</pre>

* ⚠ **WARN** This check inspects the glyph outlines and detects the total number of contours in each of them. The expected values are infered from the typical ammounts of contours observed in a large collection of reference font families. The divergences listed below may simply indicate a significantly different design on some of your glyphs. On the other hand, some of these may flag actual bugs in the font such as glyphs mapped to an incorrect codepoint. Please consider reviewing the design and codepoint assignment of these to make sure they are correct.

The following glyphs do not have the recommended number of contours:

Glyph name: at	Contours detected: 1	Expected: 2
Glyph name: Eth	Contours detected: 3	Expected: 2
Glyph name: thorn	Contours detected: 1	Expected: 2
Glyph name: aogonek	Contours detected: 3	Expected: 2
Glyph name: Dcroat	Contours detected: 3	Expected: 2
Glyph name: dcroat	Contours detected: 3	Expected: 2
Glyph name: eogonek	Contours detected: 3	Expected: 2
Glyph name: Tbar	Contours detected: 2	Expected: 1
Glyph name: Uogonek	Contours detected: 2	Expected: 1
Glyph name: uogonek	Contours detected: 2	Expected: 1
Glyph name: ohorn	Contours detected: 3	Expected: 2
Glyph name: Uhorn	Contours detected: 2	Expected: 1
Glyph name: uhorn	Contours detected: 2	Expected: 1
Glyph name: uni01EA	Contours detected: 3	Expected: 2
Glyph name: uni01EB	Contours detected: 3	Expected: 2
Glyph name: uni0203	Contours detected: 4	Expected: 3
Glyph name: uni0207	Contours detected: 4	Expected: 3
Glyph name: uni020F	Contours detected: 4	Expected: 3
Glyph name: uni0213	Contours detected: 3	Expected: 2
Glyph name: uni0217	Contours detected: 3	Expected: 2
Glyph name: uni0311	Contours detected: 2	Expected: 1
Glyph name: uni1EDB	Contours detected: 4	Expected: 3
Glyph name: uni1EDD	Contours detected: 4	Expected: 3
Glyph name: uni1EDF	Contours detected: 4	Expected: 3
Glyph name: uni1EE1	Contours detected: 4	Expected: 3
Glyph name: uni1EE3	Contours detected: 4	Expected: 3
Glyph name: uni1EE8	Contours detected: 3	Expected: 2
Glyph name: uni1EE9	Contours detected: 3	Expected: 2
Glyph name: uni1EEA	Contours detected: 3	Expected: 2
Glyph name: uni1EEB	Contours detected: 3	Expected: 2
Glyph name: uni1EEC	Contours detected: 3	Expected: 2
Glyph name: uni1EED	Contours detected: 3	Expected: 2
Glyph name: uni1EEE	Contours detected: 3	Expected: 2
Glyph name: uni1EEF	Contours detected: 3	Expected: 2
Glyph name: uni1EF0	Contours detected: 3	Expected: 2
Glyph name: uni1EF1	Contours detected: 3	Expected: 2
Glyph name: Dcroat	Contours detected: 3	Expected: 2
Glyph name: Eth	Contours detected: 3	Expected: 2
Glyph name: Tbar	Contours detected: 2	Expected: 1
Glyph name: Uhorn	Contours detected: 2	Expected: 1
Glyph name: Uogonek	Contours detected: 2	Expected: 1
Glyph name: aogonek	Contours detected: 3	Expected: 2
Glyph name: at	Contours detected: 1	Expected: 2
Glyph name: dcroat	Contours detected: 3	Expected: 2
Glyph name: eogonek	Contours detected: 3	Expected: 2
Glyph name: ohorn	Contours detected: 3	Expected: 2
Glyph name: thorn	Contours detected: 1	Expected: 2
Glyph name: uhorn	Contours detected: 2	Expected: 1
Glyph name: uni0311	Contours detected: 2	Expected: 1
Glyph name: uni1EDB	Contours detected: 4	Expected: 3
Glyph name: uni1EDD	Contours detected: 4	Expected: 3
Glyph name: uni1EDF	Contours detected: 4	Expected: 3
Glyph name: uni1EE1	Contours detected: 4	Expected: 3
Glyph name: uni1EE3	Contours detected: 4	Expected: 3
Glyph name: uni1EE8	Contours detected: 3	Expected: 2
Glyph name: uni1EE9	Contours detected: 3	Expected: 2
Glyph name: uni1EEA	Contours detected: 3	Expected: 2
Glyph name: uni1EEB	Contours detected: 3	Expected: 2
Glyph name: uni1EEC	Contours detected: 3	Expected: 2
Glyph name: uni1EED	Contours detected: 3	Expected: 2
Glyph name: uni1EEE	Contours detected: 3	Expected: 2
Glyph name: uni1EEF	Contours detected: 3	Expected: 2
Glyph name: uni1EF0	Contours detected: 3	Expected: 2
Glyph name: uni1EF1	Contours detected: 3	Expected: 2
Glyph name: uogonek	Contours detected: 2	Expected: 1 [code: contour-count]

</details>
<details>
<summary>⚠ <b>WARN:</b> Are there caret positions declared for every ligature?</summary>

* [com.google.fonts/check/ligature_carets](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/ligature_carets)
<pre>--- Rationale ---
All ligatures in a font must have corresponding caret (text cursor) positions
defined in the GDEF table, otherwhise, users may experience issues with caret
rendering.
If using GlyphsApp or UFOs, ligature carets can be defined as anchors with names
starting with &#x27;caret_&#x27;. These can be compiled with fontmake as of version
v2.4.0.</pre>

* ⚠ **WARN** This font lacks caret position values for ligature glyphs on its GDEF table. [code: lacks-caret-pos]

</details>
<details>
<summary>⚠ <b>WARN:</b> Is there kerning info for non-ligated sequences?</summary>

* [com.google.fonts/check/kerning_for_non_ligated_sequences](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/kerning_for_non_ligated_sequences)
<pre>--- Rationale ---
Fonts with ligatures should have kerning on the corresponding non-ligated
sequences for text where ligatures aren&#x27;t used (eg
https://github.com/impallari/Raleway/issues/14).</pre>

* ⚠ **WARN** GPOS table lacks kerning info for the following non-ligated sequences:
	- f + f
	- f + i
	- i + f
	- f + l
	- l + f
	- i + l

   [code: lacks-kern-info]

</details>
<details>
<summary>⚠ <b>WARN:</b> Combined length of family and style must not exceed 27 characters.</summary>

* [com.google.fonts/check/name/family_and_style_max_length](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/name/family_and_style_max_length)
<pre>--- Rationale ---
According to a GlyphsApp tutorial [1], in order to make sure all versions of
Windows recognize it as a valid font file, we must make sure that the
concatenated length of the familyname (NameID.FONT_FAMILY_NAME) and style
(NameID.FONT_SUBFAMILY_NAME) strings in the name table do not exceed 20
characters.
After discussing the problem in more detail at `FontBakery issue #2179 [2] we
decided that allowing up to 27 chars would still be on the safe side, though.
[1] https://glyphsapp.com/tutorials/multiple-masters-part-3-setting-up-instances
[2] https://github.com/googlefonts/fontbakery/issues/2179</pre>

* ⚠ **WARN** The combined length of family and style exceeds 27 chars in the following 'WINDOWS' entries:
 FONT_FAMILY_NAME = 'Foldit [Condensed,Thin]' / SUBFAMILY_NAME = 'Regular'

Please take a look at the conversation at https://github.com/googlefonts/fontbakery/issues/2179 in order to understand the reasoning behind these name table records max-length criteria. [code: too-long]

</details>
<details>
<summary>⚠ <b>WARN:</b> Ensure fonts have ScriptLangTags declared on the 'meta' table.</summary>

* [com.google.fonts/check/meta/script_lang_tags](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/meta/script_lang_tags)
<pre>--- Rationale ---
The OpenType &#x27;meta&#x27; table originated at Apple. Microsoft added it to OT with
just two DataMap records:
- dlng: comma-separated ScriptLangTags that indicate which scripts, or languages
and scripts, with possible variants, the font is designed for
- slng: comma-separated ScriptLangTags that indicate which scripts, or languages
and scripts, with possible variants, the font supports
The slng structure is intended to describe which languages and scripts the font
overall supports. For example, a Traditional Chinese font that also contains
Latin characters, can indicate Hant,Latn, showing that it supports Hant, the
Traditional Chinese variant of the Hani script, and it also supports the Latn
script
The dlng structure is far more interesting. A font may contain various glyphs,
but only a particular subset of the glyphs may be truly &quot;leading&quot; in the design,
while other glyphs may have been included for technical reasons. Such a
Traditional Chinese font could only list Hant there, showing that it’s designed
for Traditional Chinese, but the font would omit Latn, because the developers
don’t think the font is really recommended for purely Latin-script use.
The tags used in the structures can comprise just script, or also language and
script. For example, if a font has Bulgarian Cyrillic alternates in the locl
feature for the cyrl BGR OT languagesystem, it could also indicate in dlng
explicitly that it supports bul-Cyrl. (Note that the scripts and languages in
meta use the ISO language and script codes, not the OpenType ones).
This check ensures that the font has the meta table containing the slng and dlng
structures.
All families in the Google Fonts collection should contain the &#x27;meta&#x27; table.
Windows 10 already uses it when deciding on which fonts to fall back to. The
Google Fonts API and also other environments could use the data for smarter
filtering. Most importantly, those entries should be added to the Noto fonts.
In the font making process, some environments store this data in external files
already. But the meta table provides a convenient way to store this inside the
font file, so some tools may add the data, and unrelated tools may read this
data. This makes the solution much more portable and universal.</pre>

* ⚠ **WARN** This font file does not have a 'meta' table. [code: lacks-meta-table]

</details>
<details>
<summary>⚠ <b>WARN:</b> Do any segments have colinear vectors?</summary>

* [com.google.fonts/check/outline_colinear_vectors](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_colinear_vectors)
<pre>--- Rationale ---
This check looks for consecutive line segments which have the same angle. This
normally happens if an outline point has been added by accident.
This check is not run for variable fonts, as they may legitimately have colinear
vectors.</pre>

* ⚠ **WARN** The following glyphs have colinear vectors:
	* Abreve (U+0102): L<<110.0,781.0>--<91.0,803.0>> -> L<<91.0,803.0>--<60.0,839.0>>
	* Abreve (U+0102): L<<216.0,839.0>--<185.0,803.0>> -> L<<185.0,803.0>--<166.0,781.0>>
	* Ebreve (U+0114): L<<110.0,781.0>--<91.0,803.0>> -> L<<91.0,803.0>--<60.0,839.0>>
	* Ebreve (U+0114): L<<216.0,839.0>--<185.0,803.0>> -> L<<185.0,803.0>--<166.0,781.0>>
	* Gbreve (U+011E): L<<110.0,781.0>--<91.0,803.0>> -> L<<91.0,803.0>--<60.0,839.0>>
	* Gbreve (U+011E): L<<216.0,839.0>--<185.0,803.0>> -> L<<185.0,803.0>--<166.0,781.0>>
	* Ibreve (U+012C): L<<110.0,781.0>--<91.0,803.0>> -> L<<91.0,803.0>--<60.0,839.0>>
	* Ibreve (U+012C): L<<216.0,839.0>--<185.0,803.0>> -> L<<185.0,803.0>--<166.0,781.0>>
	* Lcaron (U+013D): L<<125.0,570.0>--<123.0,699.0>> -> L<<123.0,699.0>--<123.0,700.0>>
	* Obreve (U+014E): L<<110.0,781.0>--<91.0,803.0>> -> L<<91.0,803.0>--<60.0,839.0>> and 76 more. [code: found-colinear-vectors]

</details>
<details>
<summary>⚠ <b>WARN:</b> Do outlines contain any jaggy segments?</summary>

* [com.google.fonts/check/outline_jaggy_segments](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_jaggy_segments)
<pre>--- Rationale ---
This check heuristically detects outline segments which form a particularly
small angle, indicative of an outline error. This may cause false positives in
cases such as extreme ink traps, so should be regarded as advisory and backed up
by manual inspection.</pre>

* ⚠ **WARN** The following glyphs have jaggy segments:
	* M (U+004D): L<<196.0,-3.0>--<77.0,565.0>>/L<<77.0,565.0>--<77.0,0.0>> = 11.83272501030298
	* M (U+004D): L<<342.0,0.0>--<342.0,570.0>>/L<<342.0,570.0>--<222.0,-3.0>> = 11.828171622918351
	* V (U+0056): L<<77.0,700.0>--<149.0,103.0>>/L<<149.0,103.0>--<213.0,700.0>> = 12.995722982421416
	* colonmonetary (U+20A1): L<<77.0,676.0>--<77.0,263.0>>/L<<77.0,263.0>--<115.0,676.0>> = 5.256965206316971
	* oslash (U+00F8): L<<127.0,24.0>--<127.0,311.0>>/L<<127.0,311.0>--<77.0,92.0>> = 12.860793059094537
	* oslash (U+00F8): L<<77.0,476.0>--<77.0,194.0>>/L<<77.0,194.0>--<127.0,412.0>> = 12.917812843933946
	* oslashacute (U+01FF): L<<127.0,24.0>--<127.0,311.0>>/L<<127.0,311.0>--<77.0,92.0>> = 12.860793059094537
	* oslashacute (U+01FF): L<<77.0,476.0>--<77.0,194.0>>/L<<77.0,194.0>--<127.0,412.0>> = 12.917812843933946
	* zero (U+0030): L<<200.0,24.0>--<77.0,618.0>>/L<<77.0,618.0>--<77.0,24.0>> = 11.698937608802657 and zero (U+0030): L<<94.0,646.0>--<213.0,73.0>>/L<<213.0,73.0>--<213.0,646.0>> = 11.732346787462378 [code: found-jaggy-segments]

</details>
<details>
<summary>⚠ <b>WARN:</b> Do outlines contain any semi-vertical or semi-horizontal lines?</summary>

* [com.google.fonts/check/outline_semi_vertical](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_semi_vertical)
<pre>--- Rationale ---
This check detects line segments which are nearly, but not quite, exactly
horizontal or vertical. Sometimes such lines are created by design, but often
they are indicative of a design error.
This check is disabled for italic styles, which often contain nearly-upright
lines.</pre>

* ⚠ **WARN** The following glyphs have semi-vertical/semi-horizontal lines:
 * Euro (U+20AC): L<<132.0,353.0>--<252.0,354.0>>
 * Euro (U+20AC): L<<132.0,442.0>--<252.0,443.0>>
 * Euro (U+20AC): L<<275.0,330.0>--<132.0,329.0>>
 * Euro (U+20AC): L<<275.0,419.0>--<132.0,418.0>>
 * dollar (U+0024): L<<114.0,24.0>--<113.0,353.0>>
 * g (U+0067): L<<150.0,476.0>--<149.0,-177.0>>
 * gbreve (U+011F): L<<150.0,476.0>--<149.0,-177.0>>
 * gcaron (U+01E7): L<<150.0,476.0>--<149.0,-177.0>>
 * gcircumflex (U+011D): L<<150.0,476.0>--<149.0,-177.0>>
 * gdotaccent (U+0121): L<<150.0,476.0>--<149.0,-177.0>> and 18 more. [code: found-semi-vertical]

</details>
<br>
</details>
<details>
<summary><b>[22] Foldit-Fallback[Condensed,Thin].ttf</b></summary>
<details>
<summary>💔 <b>ERROR:</b> Check METADATA.pb includes production subsets.</summary>

* [com.google.fonts/check/metadata/includes_production_subsets](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/metadata/includes_production_subsets)
<pre>--- Rationale ---
Check METADATA.pb file includes the same subsets as the family in production.</pre>

* 💔 **ERROR** The condition <FontBakeryCondition:production_metadata> had an error: JSONDecodeError: Expecting value: line 1 column 1 (char 0)

</details>
<details>
<summary>💔 <b>ERROR:</b> Version number has increased since previous release on Google Fonts?</summary>

* [com.google.fonts/check/version_bump](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/version_bump)

* 💔 **ERROR** The condition <FontBakeryCondition:api_gfonts_ttFont> had an error: FailedConditionError: The condition <FontBakeryCondition:remote_styles> had an error: JSONDecodeError: Expecting value: line 1 column 1 (char 0)

</details>
<details>
<summary>💔 <b>ERROR:</b> Glyphs are similiar to Google Fonts version?</summary>

* [com.google.fonts/check/production_glyphs_similarity](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/production_glyphs_similarity)

* 💔 **ERROR** The condition <FontBakeryCondition:api_gfonts_ttFont> had an error: FailedConditionError: The condition <FontBakeryCondition:remote_styles> had an error: JSONDecodeError: Expecting value: line 1 column 1 (char 0)

</details>
<details>
<summary>💔 <b>ERROR:</b> Check if the vertical metrics of a family are similar to the same family hosted on Google Fonts.</summary>

* [com.google.fonts/check/vertical_metrics_regressions](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/vertical_metrics_regressions)
<pre>--- Rationale ---
If the family already exists on Google Fonts, we need to ensure that the checked
family&#x27;s vertical metrics are similar. This check will test the following schema
which was outlined in Fontbakery issue #1162 [1]:
- The family should visually have the same vertical metrics as the Regular style
hosted on Google Fonts.
- If the family on Google Fonts has differing hhea and typo metrics, the family
being checked should use the typo metrics for both the hhea and typo entries.
- If the family on Google Fonts has use typo metrics not enabled and the family
being checked has it enabled, the hhea and typo metrics should use the family on
Google Fonts winAscent and winDescent values.
- If the upms differ, the values must be scaled so the visual appearance is the
same.
[1] https://github.com/googlefonts/fontbakery/issues/1162</pre>

* 💔 **ERROR** The condition <FontBakeryCondition:regular_remote_style> had an error: FailedConditionError: The condition <FontBakeryCondition:remote_styles> had an error: JSONDecodeError: Expecting value: line 1 column 1 (char 0)

</details>
<details>
<summary>💔 <b>ERROR:</b> Check font follows the Google Fonts CJK vertical metric schema</summary>

* [com.google.fonts/check/cjk_vertical_metrics](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/cjk_vertical_metrics)
<pre>--- Rationale ---
CJK fonts have different vertical metrics when compared to Latin fonts. We
follow the schema developed by dr Ken Lunde for Source Han Sans and the Noto CJK
fonts.
Our documentation includes further information:
https://github.com/googlefonts/gf-docs/tree/main/Spec#cjk-vertical-metrics</pre>

* 💔 **ERROR** The condition <FontBakeryCondition:remote_styles> had an error: JSONDecodeError: Expecting value: line 1 column 1 (char 0)

</details>
<details>
<summary>💔 <b>ERROR:</b> Check if the vertical metrics of a CJK family are similar to the same family hosted on Google Fonts.</summary>

* [com.google.fonts/check/cjk_vertical_metrics_regressions](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/cjk_vertical_metrics_regressions)
<pre>--- Rationale ---
Check CJK family has the same vertical metrics as the same family hosted on
Google Fonts.</pre>

* 💔 **ERROR** The condition <FontBakeryCondition:regular_remote_style> had an error: FailedConditionError: The condition <FontBakeryCondition:remote_styles> had an error: JSONDecodeError: Expecting value: line 1 column 1 (char 0)

</details>
<details>
<summary>🔥 <b>FAIL:</b> Checking file is named canonically.</summary>

* [com.google.fonts/check/canonical_filename](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/canonical_filename)
<pre>--- Rationale ---
A font&#x27;s filename must be composed in the following manner:
&lt;familyname&gt;-&lt;stylename&gt;.ttf
- Nunito-Regular.ttf,
- Oswald-BoldItalic.ttf
Variable fonts must list the axis tags in alphabetical order in square brackets
and separated by commas:
- Roboto[wdth,wght].ttf
- Familyname-Italic[wght].ttf</pre>

* 🔥 **FAIL** Style name used in "fonts/ttf/Foldit-Fallback[Condensed,Thin].ttf" is not canonical. You should rebuild the font using any of the following style names: "Thin", "ExtraLight", "Light", "Regular", "Medium", "SemiBold", "Bold", "ExtraBold", "Black", "Thin Italic", "ExtraLight Italic", "Light Italic", "Italic", "Medium Italic", "SemiBold Italic", "Bold Italic", "ExtraBold Italic", "Black Italic". [code: bad-static-filename]

</details>
<details>
<summary>🔥 <b>FAIL:</b> Check `Google Fonts Latin Core` glyph coverage.</summary>

* [com.google.fonts/check/glyph_coverage](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/glyph_coverage)
<pre>--- Rationale ---
Google Fonts expects that fonts in its collection support at least the minimal
set of characters defined in the `GF-latin-core` glyph-set.</pre>

* 🔥 **FAIL** Missing required codepoints: 0x00A0 (NO-BREAK SPACE) [code: missing-codepoints]

</details>
<details>
<summary>🔥 <b>FAIL:</b> Check copyright namerecords match license file.</summary>

* [com.google.fonts/check/name/license](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/name/license)
<pre>--- Rationale ---
A known licensing description must be provided in the NameID 14 (LICENSE
DESCRIPTION) entries of the name table.
The source of truth for this check (to determine which license is in use) is a
file placed side-by-side to your font project including the licensing terms.
Depending on the chosen license, one of the following string snippets is
expected to be found on the NameID 13 (LICENSE DESCRIPTION) entries of the name
table:
- &quot;This Font Software is licensed under the SIL Open Font License, Version 1.1.
This license is available with a FAQ at: https://scripts.sil.org/OFL&quot;
- &quot;Licensed under the Apache License, Version 2.0&quot;
- &quot;Licensed under the Ubuntu Font Licence 1.0.&quot;
Currently accepted licenses are Apache or Open Font License.
For a small set of legacy families the Ubuntu Font License may be acceptable as
well.
When in doubt, please choose OFL for new font projects.</pre>

* 🔥 **FAIL** License file OFL.txt exists but NameID 13 (LICENSE DESCRIPTION) value on platform 3 (WINDOWS) is not specified for that. Value was: "This Font Software is licensed under the SIL Open Font License, Version 1.1. This license..." Must be changed to "This Font Software is licensed under the SIL Open Font License, Version 1.1. This license is available with a FAQ at: https://scripts.sil.org/OFL" [code: wrong]

</details>
<details>
<summary>🔥 <b>FAIL:</b> Check name table: TYPOGRAPHIC_SUBFAMILY_NAME entries.</summary>

* [com.google.fonts/check/name/typographicsubfamilyname](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/name/typographicsubfamilyname)
<pre>--- Rationale ---
Requirements for the TYPOGRAPHIC_SUBFAMILY_NAME entries in the &#x27;name&#x27; table.</pre>

* 🔥 **FAIL** TYPOGRAPHIC_SUBFAMILY_NAME for Win "Fallback[Condensed,Thin]" is incorrect. It must be "Thin". [code: bad-typo-win]

</details>
<details>
<summary>🔥 <b>FAIL:</b> Checking OS/2 usWinAscent & usWinDescent.</summary>

* [com.google.fonts/check/family/win_ascent_and_descent](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/universal.html#com.google.fonts/check/family/win_ascent_and_descent)
<pre>--- Rationale ---
A font&#x27;s winAscent and winDescent values should be greater than the head table&#x27;s
yMax, abs(yMin) values. If they are less than these values, clipping can occur
on Windows platforms (https://github.com/RedHatBrand/Overpass/issues/33).
If the font includes tall/deep writing systems such as Arabic or Devanagari, the
winAscent and winDescent can be greater than the yMax and abs(yMin) to
accommodate vowel marks.
When the win Metrics are significantly greater than the upm, the linespacing can
appear too loose. To counteract this, enabling the OS/2 fsSelection bit 7
(Use_Typo_Metrics), will force Windows to use the OS/2 typo values instead. This
means the font developer can control the linespacing with the typo values,
whilst avoiding clipping by setting the win values to values greater than the
yMax and abs(yMin).</pre>

* 🔥 **FAIL** OS/2.usWinAscent value should be equal or greater than 1029, but got 800 instead [code: ascent]
* 🔥 **FAIL** OS/2.usWinDescent value should be equal or greater than 268, but got 200 instead. [code: descent]

</details>
<details>
<summary>🔥 <b>FAIL:</b> Font contains glyphs for whitespace characters?</summary>

* [com.google.fonts/check/whitespace_glyphs](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/universal.html#com.google.fonts/check/whitespace_glyphs)

* 🔥 **FAIL** Whitespace glyph missing for codepoint 0x00A0. [code: missing-whitespace-glyph-0x00A0]

</details>
<details>
<summary>⚠ <b>WARN:</b> Checking OS/2 achVendID.</summary>

* [com.google.fonts/check/vendor_id](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/vendor_id)
<pre>--- Rationale ---
Microsoft keeps a list of font vendors and their respective contact info. This
list is updated regularly and is indexed by a 4-char &quot;Vendor ID&quot; which is stored
in the achVendID field of the OS/2 table.
Registering your ID is not mandatory, but it is a good practice since some
applications may display the type designer / type foundry contact info on some
dialog and also because that info will be visible on Microsoft&#x27;s website:
https://docs.microsoft.com/en-us/typography/vendors/
This check verifies whether or not a given font&#x27;s vendor ID is registered in
that list or if it has some of the default values used by the most common font
editors.
Each new FontBakery release includes a cached copy of that list of vendor IDs.
If you registered recently, you&#x27;re safe to ignore warnings emitted by this
check, since your ID will soon be included in one of our upcoming releases.</pre>

* ⚠ **WARN** OS/2 VendorID value 'NONE' is not yet recognized. If you registered it recently, then it's safe to ignore this warning message. Otherwise, you should set it to your own unique 4 character code, and register it with Microsoft at https://www.microsoft.com/typography/links/vendorlist.aspx
 [code: unknown]

</details>
<details>
<summary>⚠ <b>WARN:</b> Font has old ttfautohint applied?</summary>

* [com.google.fonts/check/old_ttfautohint](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/old_ttfautohint)
<pre>--- Rationale ---
Check if font has been hinted with an outdated version of ttfautohint.</pre>

* ⚠ **WARN** ttfautohint used in font = 1.8.3; latest = 1.8.4; Need to re-run with the newer version! [code: old-ttfa]

</details>
<details>
<summary>⚠ <b>WARN:</b> Check if each glyph has the recommended amount of contours.</summary>

* [com.google.fonts/check/contour_count](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/contour_count)
<pre>--- Rationale ---
Visually QAing thousands of glyphs by hand is tiring. Most glyphs can only be
constructured in a handful of ways. This means a glyph&#x27;s contour count will only
differ slightly amongst different fonts, e.g a &#x27;g&#x27; could either be 2 or 3
contours, depending on whether its double story or single story.
However, a quotedbl should have 2 contours, unless the font belongs to a display
family.
This check currently does not cover variable fonts because there&#x27;s plenty of
alternative ways of constructing glyphs with multiple outlines for each feature
in a VarFont. The expected contour count data for this check is currently
optimized for the typical construction of glyphs in static fonts.</pre>

* ⚠ **WARN** This check inspects the glyph outlines and detects the total number of contours in each of them. The expected values are infered from the typical ammounts of contours observed in a large collection of reference font families. The divergences listed below may simply indicate a significantly different design on some of your glyphs. On the other hand, some of these may flag actual bugs in the font such as glyphs mapped to an incorrect codepoint. Please consider reviewing the design and codepoint assignment of these to make sure they are correct.

The following glyphs do not have the recommended number of contours:

Glyph name: at	Contours detected: 1	Expected: 2
Glyph name: Eth	Contours detected: 3	Expected: 2
Glyph name: thorn	Contours detected: 1	Expected: 2
Glyph name: aogonek	Contours detected: 3	Expected: 2
Glyph name: Dcroat	Contours detected: 3	Expected: 2
Glyph name: dcroat	Contours detected: 3	Expected: 2
Glyph name: eogonek	Contours detected: 3	Expected: 2
Glyph name: Tbar	Contours detected: 2	Expected: 1
Glyph name: Uogonek	Contours detected: 2	Expected: 1
Glyph name: uogonek	Contours detected: 2	Expected: 1
Glyph name: ohorn	Contours detected: 3	Expected: 2
Glyph name: Uhorn	Contours detected: 2	Expected: 1
Glyph name: uhorn	Contours detected: 2	Expected: 1
Glyph name: uni01EA	Contours detected: 3	Expected: 2
Glyph name: uni01EB	Contours detected: 3	Expected: 2
Glyph name: uni0203	Contours detected: 4	Expected: 3
Glyph name: uni0207	Contours detected: 4	Expected: 3
Glyph name: uni020F	Contours detected: 4	Expected: 3
Glyph name: uni0213	Contours detected: 3	Expected: 2
Glyph name: uni0217	Contours detected: 3	Expected: 2
Glyph name: uni0311	Contours detected: 2	Expected: 1
Glyph name: uni1EDB	Contours detected: 4	Expected: 3
Glyph name: uni1EDD	Contours detected: 4	Expected: 3
Glyph name: uni1EDF	Contours detected: 4	Expected: 3
Glyph name: uni1EE1	Contours detected: 4	Expected: 3
Glyph name: uni1EE3	Contours detected: 4	Expected: 3
Glyph name: uni1EE8	Contours detected: 3	Expected: 2
Glyph name: uni1EE9	Contours detected: 3	Expected: 2
Glyph name: uni1EEA	Contours detected: 3	Expected: 2
Glyph name: uni1EEB	Contours detected: 3	Expected: 2
Glyph name: uni1EEC	Contours detected: 3	Expected: 2
Glyph name: uni1EED	Contours detected: 3	Expected: 2
Glyph name: uni1EEE	Contours detected: 3	Expected: 2
Glyph name: uni1EEF	Contours detected: 3	Expected: 2
Glyph name: uni1EF0	Contours detected: 3	Expected: 2
Glyph name: uni1EF1	Contours detected: 3	Expected: 2
Glyph name: Dcroat	Contours detected: 3	Expected: 2
Glyph name: Eth	Contours detected: 3	Expected: 2
Glyph name: Tbar	Contours detected: 2	Expected: 1
Glyph name: Uhorn	Contours detected: 2	Expected: 1
Glyph name: Uogonek	Contours detected: 2	Expected: 1
Glyph name: aogonek	Contours detected: 3	Expected: 2
Glyph name: at	Contours detected: 1	Expected: 2
Glyph name: dcroat	Contours detected: 3	Expected: 2
Glyph name: eogonek	Contours detected: 3	Expected: 2
Glyph name: ohorn	Contours detected: 3	Expected: 2
Glyph name: thorn	Contours detected: 1	Expected: 2
Glyph name: uhorn	Contours detected: 2	Expected: 1
Glyph name: uni0311	Contours detected: 2	Expected: 1
Glyph name: uni1EDB	Contours detected: 4	Expected: 3
Glyph name: uni1EDD	Contours detected: 4	Expected: 3
Glyph name: uni1EDF	Contours detected: 4	Expected: 3
Glyph name: uni1EE1	Contours detected: 4	Expected: 3
Glyph name: uni1EE3	Contours detected: 4	Expected: 3
Glyph name: uni1EE8	Contours detected: 3	Expected: 2
Glyph name: uni1EE9	Contours detected: 3	Expected: 2
Glyph name: uni1EEA	Contours detected: 3	Expected: 2
Glyph name: uni1EEB	Contours detected: 3	Expected: 2
Glyph name: uni1EEC	Contours detected: 3	Expected: 2
Glyph name: uni1EED	Contours detected: 3	Expected: 2
Glyph name: uni1EEE	Contours detected: 3	Expected: 2
Glyph name: uni1EEF	Contours detected: 3	Expected: 2
Glyph name: uni1EF0	Contours detected: 3	Expected: 2
Glyph name: uni1EF1	Contours detected: 3	Expected: 2
Glyph name: uogonek	Contours detected: 2	Expected: 1 [code: contour-count]

</details>
<details>
<summary>⚠ <b>WARN:</b> Are there caret positions declared for every ligature?</summary>

* [com.google.fonts/check/ligature_carets](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/ligature_carets)
<pre>--- Rationale ---
All ligatures in a font must have corresponding caret (text cursor) positions
defined in the GDEF table, otherwhise, users may experience issues with caret
rendering.
If using GlyphsApp or UFOs, ligature carets can be defined as anchors with names
starting with &#x27;caret_&#x27;. These can be compiled with fontmake as of version
v2.4.0.</pre>

* ⚠ **WARN** This font lacks caret position values for ligature glyphs on its GDEF table. [code: lacks-caret-pos]

</details>
<details>
<summary>⚠ <b>WARN:</b> Is there kerning info for non-ligated sequences?</summary>

* [com.google.fonts/check/kerning_for_non_ligated_sequences](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/kerning_for_non_ligated_sequences)
<pre>--- Rationale ---
Fonts with ligatures should have kerning on the corresponding non-ligated
sequences for text where ligatures aren&#x27;t used (eg
https://github.com/impallari/Raleway/issues/14).</pre>

* ⚠ **WARN** GPOS table lacks kerning info for the following non-ligated sequences:
	- f + f
	- f + i
	- i + f
	- f + l
	- l + f
	- i + l

   [code: lacks-kern-info]

</details>
<details>
<summary>⚠ <b>WARN:</b> Combined length of family and style must not exceed 27 characters.</summary>

* [com.google.fonts/check/name/family_and_style_max_length](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/name/family_and_style_max_length)
<pre>--- Rationale ---
According to a GlyphsApp tutorial [1], in order to make sure all versions of
Windows recognize it as a valid font file, we must make sure that the
concatenated length of the familyname (NameID.FONT_FAMILY_NAME) and style
(NameID.FONT_SUBFAMILY_NAME) strings in the name table do not exceed 20
characters.
After discussing the problem in more detail at `FontBakery issue #2179 [2] we
decided that allowing up to 27 chars would still be on the safe side, though.
[1] https://glyphsapp.com/tutorials/multiple-masters-part-3-setting-up-instances
[2] https://github.com/googlefonts/fontbakery/issues/2179</pre>

* ⚠ **WARN** The combined length of family and style exceeds 27 chars in the following 'WINDOWS' entries:
 FONT_FAMILY_NAME = 'Foldit Fallback[Condensed,Thin]' / SUBFAMILY_NAME = 'Regular'

Please take a look at the conversation at https://github.com/googlefonts/fontbakery/issues/2179 in order to understand the reasoning behind these name table records max-length criteria. [code: too-long]

</details>
<details>
<summary>⚠ <b>WARN:</b> Ensure fonts have ScriptLangTags declared on the 'meta' table.</summary>

* [com.google.fonts/check/meta/script_lang_tags](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/meta/script_lang_tags)
<pre>--- Rationale ---
The OpenType &#x27;meta&#x27; table originated at Apple. Microsoft added it to OT with
just two DataMap records:
- dlng: comma-separated ScriptLangTags that indicate which scripts, or languages
and scripts, with possible variants, the font is designed for
- slng: comma-separated ScriptLangTags that indicate which scripts, or languages
and scripts, with possible variants, the font supports
The slng structure is intended to describe which languages and scripts the font
overall supports. For example, a Traditional Chinese font that also contains
Latin characters, can indicate Hant,Latn, showing that it supports Hant, the
Traditional Chinese variant of the Hani script, and it also supports the Latn
script
The dlng structure is far more interesting. A font may contain various glyphs,
but only a particular subset of the glyphs may be truly &quot;leading&quot; in the design,
while other glyphs may have been included for technical reasons. Such a
Traditional Chinese font could only list Hant there, showing that it’s designed
for Traditional Chinese, but the font would omit Latn, because the developers
don’t think the font is really recommended for purely Latin-script use.
The tags used in the structures can comprise just script, or also language and
script. For example, if a font has Bulgarian Cyrillic alternates in the locl
feature for the cyrl BGR OT languagesystem, it could also indicate in dlng
explicitly that it supports bul-Cyrl. (Note that the scripts and languages in
meta use the ISO language and script codes, not the OpenType ones).
This check ensures that the font has the meta table containing the slng and dlng
structures.
All families in the Google Fonts collection should contain the &#x27;meta&#x27; table.
Windows 10 already uses it when deciding on which fonts to fall back to. The
Google Fonts API and also other environments could use the data for smarter
filtering. Most importantly, those entries should be added to the Noto fonts.
In the font making process, some environments store this data in external files
already. But the meta table provides a convenient way to store this inside the
font file, so some tools may add the data, and unrelated tools may read this
data. This makes the solution much more portable and universal.</pre>

* ⚠ **WARN** This font file does not have a 'meta' table. [code: lacks-meta-table]

</details>
<details>
<summary>⚠ <b>WARN:</b> Do any segments have colinear vectors?</summary>

* [com.google.fonts/check/outline_colinear_vectors](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_colinear_vectors)
<pre>--- Rationale ---
This check looks for consecutive line segments which have the same angle. This
normally happens if an outline point has been added by accident.
This check is not run for variable fonts, as they may legitimately have colinear
vectors.</pre>

* ⚠ **WARN** The following glyphs have colinear vectors:
	* Abreve (U+0102): L<<110.0,781.0>--<91.0,803.0>> -> L<<91.0,803.0>--<60.0,839.0>>
	* Abreve (U+0102): L<<216.0,839.0>--<185.0,803.0>> -> L<<185.0,803.0>--<166.0,781.0>>
	* Ebreve (U+0114): L<<110.0,781.0>--<91.0,803.0>> -> L<<91.0,803.0>--<60.0,839.0>>
	* Ebreve (U+0114): L<<216.0,839.0>--<185.0,803.0>> -> L<<185.0,803.0>--<166.0,781.0>>
	* Gbreve (U+011E): L<<110.0,781.0>--<91.0,803.0>> -> L<<91.0,803.0>--<60.0,839.0>>
	* Gbreve (U+011E): L<<216.0,839.0>--<185.0,803.0>> -> L<<185.0,803.0>--<166.0,781.0>>
	* Ibreve (U+012C): L<<110.0,781.0>--<91.0,803.0>> -> L<<91.0,803.0>--<60.0,839.0>>
	* Ibreve (U+012C): L<<216.0,839.0>--<185.0,803.0>> -> L<<185.0,803.0>--<166.0,781.0>>
	* Lcaron (U+013D): L<<125.0,570.0>--<123.0,699.0>> -> L<<123.0,699.0>--<123.0,700.0>>
	* Obreve (U+014E): L<<110.0,781.0>--<91.0,803.0>> -> L<<91.0,803.0>--<60.0,839.0>> and 76 more. [code: found-colinear-vectors]

</details>
<details>
<summary>⚠ <b>WARN:</b> Do outlines contain any jaggy segments?</summary>

* [com.google.fonts/check/outline_jaggy_segments](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_jaggy_segments)
<pre>--- Rationale ---
This check heuristically detects outline segments which form a particularly
small angle, indicative of an outline error. This may cause false positives in
cases such as extreme ink traps, so should be regarded as advisory and backed up
by manual inspection.</pre>

* ⚠ **WARN** The following glyphs have jaggy segments:
	* M (U+004D): L<<196.0,-3.0>--<77.0,565.0>>/L<<77.0,565.0>--<77.0,0.0>> = 11.83272501030298
	* M (U+004D): L<<342.0,0.0>--<342.0,570.0>>/L<<342.0,570.0>--<222.0,-3.0>> = 11.828171622918351
	* V (U+0056): L<<77.0,700.0>--<149.0,103.0>>/L<<149.0,103.0>--<213.0,700.0>> = 12.995722982421416
	* colonmonetary (U+20A1): L<<77.0,676.0>--<77.0,263.0>>/L<<77.0,263.0>--<115.0,676.0>> = 5.256965206316971
	* oslash (U+00F8): L<<127.0,24.0>--<127.0,311.0>>/L<<127.0,311.0>--<77.0,92.0>> = 12.860793059094537
	* oslash (U+00F8): L<<77.0,476.0>--<77.0,194.0>>/L<<77.0,194.0>--<127.0,412.0>> = 12.917812843933946
	* oslashacute (U+01FF): L<<127.0,24.0>--<127.0,311.0>>/L<<127.0,311.0>--<77.0,92.0>> = 12.860793059094537
	* oslashacute (U+01FF): L<<77.0,476.0>--<77.0,194.0>>/L<<77.0,194.0>--<127.0,412.0>> = 12.917812843933946
	* zero (U+0030): L<<200.0,24.0>--<77.0,618.0>>/L<<77.0,618.0>--<77.0,24.0>> = 11.698937608802657 and zero (U+0030): L<<94.0,646.0>--<213.0,73.0>>/L<<213.0,73.0>--<213.0,646.0>> = 11.732346787462378 [code: found-jaggy-segments]

</details>
<details>
<summary>⚠ <b>WARN:</b> Do outlines contain any semi-vertical or semi-horizontal lines?</summary>

* [com.google.fonts/check/outline_semi_vertical](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_semi_vertical)
<pre>--- Rationale ---
This check detects line segments which are nearly, but not quite, exactly
horizontal or vertical. Sometimes such lines are created by design, but often
they are indicative of a design error.
This check is disabled for italic styles, which often contain nearly-upright
lines.</pre>

* ⚠ **WARN** The following glyphs have semi-vertical/semi-horizontal lines:
 * Euro (U+20AC): L<<132.0,353.0>--<252.0,354.0>>
 * Euro (U+20AC): L<<132.0,442.0>--<252.0,443.0>>
 * Euro (U+20AC): L<<275.0,330.0>--<132.0,329.0>>
 * Euro (U+20AC): L<<275.0,419.0>--<132.0,418.0>>
 * dollar (U+0024): L<<114.0,24.0>--<113.0,353.0>>
 * g (U+0067): L<<150.0,476.0>--<149.0,-177.0>>
 * gbreve (U+011F): L<<150.0,476.0>--<149.0,-177.0>>
 * gcaron (U+01E7): L<<150.0,476.0>--<149.0,-177.0>>
 * gcircumflex (U+011D): L<<150.0,476.0>--<149.0,-177.0>>
 * gdotaccent (U+0121): L<<150.0,476.0>--<149.0,-177.0>> and 18 more. [code: found-semi-vertical]

</details>
<br>
</details>
<details>
<summary><b>[21] Foldit-Fallback[Expanded,ExtraBold].ttf</b></summary>
<details>
<summary>💔 <b>ERROR:</b> Check METADATA.pb includes production subsets.</summary>

* [com.google.fonts/check/metadata/includes_production_subsets](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/metadata/includes_production_subsets)
<pre>--- Rationale ---
Check METADATA.pb file includes the same subsets as the family in production.</pre>

* 💔 **ERROR** The condition <FontBakeryCondition:production_metadata> had an error: JSONDecodeError: Expecting value: line 1 column 1 (char 0)

</details>
<details>
<summary>💔 <b>ERROR:</b> Version number has increased since previous release on Google Fonts?</summary>

* [com.google.fonts/check/version_bump](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/version_bump)

* 💔 **ERROR** The condition <FontBakeryCondition:api_gfonts_ttFont> had an error: FailedConditionError: The condition <FontBakeryCondition:remote_styles> had an error: JSONDecodeError: Expecting value: line 1 column 1 (char 0)

</details>
<details>
<summary>💔 <b>ERROR:</b> Glyphs are similiar to Google Fonts version?</summary>

* [com.google.fonts/check/production_glyphs_similarity](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/production_glyphs_similarity)

* 💔 **ERROR** The condition <FontBakeryCondition:api_gfonts_ttFont> had an error: FailedConditionError: The condition <FontBakeryCondition:remote_styles> had an error: JSONDecodeError: Expecting value: line 1 column 1 (char 0)

</details>
<details>
<summary>💔 <b>ERROR:</b> Check if the vertical metrics of a family are similar to the same family hosted on Google Fonts.</summary>

* [com.google.fonts/check/vertical_metrics_regressions](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/vertical_metrics_regressions)
<pre>--- Rationale ---
If the family already exists on Google Fonts, we need to ensure that the checked
family&#x27;s vertical metrics are similar. This check will test the following schema
which was outlined in Fontbakery issue #1162 [1]:
- The family should visually have the same vertical metrics as the Regular style
hosted on Google Fonts.
- If the family on Google Fonts has differing hhea and typo metrics, the family
being checked should use the typo metrics for both the hhea and typo entries.
- If the family on Google Fonts has use typo metrics not enabled and the family
being checked has it enabled, the hhea and typo metrics should use the family on
Google Fonts winAscent and winDescent values.
- If the upms differ, the values must be scaled so the visual appearance is the
same.
[1] https://github.com/googlefonts/fontbakery/issues/1162</pre>

* 💔 **ERROR** The condition <FontBakeryCondition:regular_remote_style> had an error: FailedConditionError: The condition <FontBakeryCondition:remote_styles> had an error: JSONDecodeError: Expecting value: line 1 column 1 (char 0)

</details>
<details>
<summary>💔 <b>ERROR:</b> Check font follows the Google Fonts CJK vertical metric schema</summary>

* [com.google.fonts/check/cjk_vertical_metrics](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/cjk_vertical_metrics)
<pre>--- Rationale ---
CJK fonts have different vertical metrics when compared to Latin fonts. We
follow the schema developed by dr Ken Lunde for Source Han Sans and the Noto CJK
fonts.
Our documentation includes further information:
https://github.com/googlefonts/gf-docs/tree/main/Spec#cjk-vertical-metrics</pre>

* 💔 **ERROR** The condition <FontBakeryCondition:remote_styles> had an error: JSONDecodeError: Expecting value: line 1 column 1 (char 0)

</details>
<details>
<summary>💔 <b>ERROR:</b> Check if the vertical metrics of a CJK family are similar to the same family hosted on Google Fonts.</summary>

* [com.google.fonts/check/cjk_vertical_metrics_regressions](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/cjk_vertical_metrics_regressions)
<pre>--- Rationale ---
Check CJK family has the same vertical metrics as the same family hosted on
Google Fonts.</pre>

* 💔 **ERROR** The condition <FontBakeryCondition:regular_remote_style> had an error: FailedConditionError: The condition <FontBakeryCondition:remote_styles> had an error: JSONDecodeError: Expecting value: line 1 column 1 (char 0)

</details>
<details>
<summary>🔥 <b>FAIL:</b> Checking file is named canonically.</summary>

* [com.google.fonts/check/canonical_filename](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/canonical_filename)
<pre>--- Rationale ---
A font&#x27;s filename must be composed in the following manner:
&lt;familyname&gt;-&lt;stylename&gt;.ttf
- Nunito-Regular.ttf,
- Oswald-BoldItalic.ttf
Variable fonts must list the axis tags in alphabetical order in square brackets
and separated by commas:
- Roboto[wdth,wght].ttf
- Familyname-Italic[wght].ttf</pre>

* 🔥 **FAIL** Style name used in "fonts/ttf/Foldit-Fallback[Expanded,ExtraBold].ttf" is not canonical. You should rebuild the font using any of the following style names: "Thin", "ExtraLight", "Light", "Regular", "Medium", "SemiBold", "Bold", "ExtraBold", "Black", "Thin Italic", "ExtraLight Italic", "Light Italic", "Italic", "Medium Italic", "SemiBold Italic", "Bold Italic", "ExtraBold Italic", "Black Italic". [code: bad-static-filename]

</details>
<details>
<summary>🔥 <b>FAIL:</b> Check `Google Fonts Latin Core` glyph coverage.</summary>

* [com.google.fonts/check/glyph_coverage](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/glyph_coverage)
<pre>--- Rationale ---
Google Fonts expects that fonts in its collection support at least the minimal
set of characters defined in the `GF-latin-core` glyph-set.</pre>

* 🔥 **FAIL** Missing required codepoints: 0x00A0 (NO-BREAK SPACE) [code: missing-codepoints]

</details>
<details>
<summary>🔥 <b>FAIL:</b> Check copyright namerecords match license file.</summary>

* [com.google.fonts/check/name/license](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/name/license)
<pre>--- Rationale ---
A known licensing description must be provided in the NameID 14 (LICENSE
DESCRIPTION) entries of the name table.
The source of truth for this check (to determine which license is in use) is a
file placed side-by-side to your font project including the licensing terms.
Depending on the chosen license, one of the following string snippets is
expected to be found on the NameID 13 (LICENSE DESCRIPTION) entries of the name
table:
- &quot;This Font Software is licensed under the SIL Open Font License, Version 1.1.
This license is available with a FAQ at: https://scripts.sil.org/OFL&quot;
- &quot;Licensed under the Apache License, Version 2.0&quot;
- &quot;Licensed under the Ubuntu Font Licence 1.0.&quot;
Currently accepted licenses are Apache or Open Font License.
For a small set of legacy families the Ubuntu Font License may be acceptable as
well.
When in doubt, please choose OFL for new font projects.</pre>

* 🔥 **FAIL** License file OFL.txt exists but NameID 13 (LICENSE DESCRIPTION) value on platform 3 (WINDOWS) is not specified for that. Value was: "This Font Software is licensed under the SIL Open Font License, Version 1.1. This license..." Must be changed to "This Font Software is licensed under the SIL Open Font License, Version 1.1. This license is available with a FAQ at: https://scripts.sil.org/OFL" [code: wrong]

</details>
<details>
<summary>🔥 <b>FAIL:</b> Check name table: TYPOGRAPHIC_SUBFAMILY_NAME entries.</summary>

* [com.google.fonts/check/name/typographicsubfamilyname](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/name/typographicsubfamilyname)
<pre>--- Rationale ---
Requirements for the TYPOGRAPHIC_SUBFAMILY_NAME entries in the &#x27;name&#x27; table.</pre>

* 🔥 **FAIL** TYPOGRAPHIC_SUBFAMILY_NAME for Win "Fallback[Expanded,ExtraBold]" is incorrect. It must be "ExtraBold". [code: bad-typo-win]

</details>
<details>
<summary>🔥 <b>FAIL:</b> Checking OS/2 usWinAscent & usWinDescent.</summary>

* [com.google.fonts/check/family/win_ascent_and_descent](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/universal.html#com.google.fonts/check/family/win_ascent_and_descent)
<pre>--- Rationale ---
A font&#x27;s winAscent and winDescent values should be greater than the head table&#x27;s
yMax, abs(yMin) values. If they are less than these values, clipping can occur
on Windows platforms (https://github.com/RedHatBrand/Overpass/issues/33).
If the font includes tall/deep writing systems such as Arabic or Devanagari, the
winAscent and winDescent can be greater than the yMax and abs(yMin) to
accommodate vowel marks.
When the win Metrics are significantly greater than the upm, the linespacing can
appear too loose. To counteract this, enabling the OS/2 fsSelection bit 7
(Use_Typo_Metrics), will force Windows to use the OS/2 typo values instead. This
means the font developer can control the linespacing with the typo values,
whilst avoiding clipping by setting the win values to values greater than the
yMax and abs(yMin).</pre>

* 🔥 **FAIL** OS/2.usWinAscent value should be equal or greater than 1029, but got 800 instead [code: ascent]
* 🔥 **FAIL** OS/2.usWinDescent value should be equal or greater than 268, but got 200 instead. [code: descent]

</details>
<details>
<summary>🔥 <b>FAIL:</b> Font contains glyphs for whitespace characters?</summary>

* [com.google.fonts/check/whitespace_glyphs](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/universal.html#com.google.fonts/check/whitespace_glyphs)

* 🔥 **FAIL** Whitespace glyph missing for codepoint 0x00A0. [code: missing-whitespace-glyph-0x00A0]

</details>
<details>
<summary>⚠ <b>WARN:</b> Checking OS/2 achVendID.</summary>

* [com.google.fonts/check/vendor_id](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/vendor_id)
<pre>--- Rationale ---
Microsoft keeps a list of font vendors and their respective contact info. This
list is updated regularly and is indexed by a 4-char &quot;Vendor ID&quot; which is stored
in the achVendID field of the OS/2 table.
Registering your ID is not mandatory, but it is a good practice since some
applications may display the type designer / type foundry contact info on some
dialog and also because that info will be visible on Microsoft&#x27;s website:
https://docs.microsoft.com/en-us/typography/vendors/
This check verifies whether or not a given font&#x27;s vendor ID is registered in
that list or if it has some of the default values used by the most common font
editors.
Each new FontBakery release includes a cached copy of that list of vendor IDs.
If you registered recently, you&#x27;re safe to ignore warnings emitted by this
check, since your ID will soon be included in one of our upcoming releases.</pre>

* ⚠ **WARN** OS/2 VendorID value 'NONE' is not yet recognized. If you registered it recently, then it's safe to ignore this warning message. Otherwise, you should set it to your own unique 4 character code, and register it with Microsoft at https://www.microsoft.com/typography/links/vendorlist.aspx
 [code: unknown]

</details>
<details>
<summary>⚠ <b>WARN:</b> Font has old ttfautohint applied?</summary>

* [com.google.fonts/check/old_ttfautohint](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/old_ttfautohint)
<pre>--- Rationale ---
Check if font has been hinted with an outdated version of ttfautohint.</pre>

* ⚠ **WARN** ttfautohint used in font = 1.8.3; latest = 1.8.4; Need to re-run with the newer version! [code: old-ttfa]

</details>
<details>
<summary>⚠ <b>WARN:</b> Check if each glyph has the recommended amount of contours.</summary>

* [com.google.fonts/check/contour_count](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/contour_count)
<pre>--- Rationale ---
Visually QAing thousands of glyphs by hand is tiring. Most glyphs can only be
constructured in a handful of ways. This means a glyph&#x27;s contour count will only
differ slightly amongst different fonts, e.g a &#x27;g&#x27; could either be 2 or 3
contours, depending on whether its double story or single story.
However, a quotedbl should have 2 contours, unless the font belongs to a display
family.
This check currently does not cover variable fonts because there&#x27;s plenty of
alternative ways of constructing glyphs with multiple outlines for each feature
in a VarFont. The expected contour count data for this check is currently
optimized for the typical construction of glyphs in static fonts.</pre>

* ⚠ **WARN** This check inspects the glyph outlines and detects the total number of contours in each of them. The expected values are infered from the typical ammounts of contours observed in a large collection of reference font families. The divergences listed below may simply indicate a significantly different design on some of your glyphs. On the other hand, some of these may flag actual bugs in the font such as glyphs mapped to an incorrect codepoint. Please consider reviewing the design and codepoint assignment of these to make sure they are correct.

The following glyphs do not have the recommended number of contours:

Glyph name: one	Contours detected: 2	Expected: 1
Glyph name: at	Contours detected: 1	Expected: 2
Glyph name: I	Contours detected: 2	Expected: 1
Glyph name: y	Contours detected: 2	Expected: 1
Glyph name: uni00B9	Contours detected: 2	Expected: 1
Glyph name: onehalf	Contours detected: 4	Expected: 3
Glyph name: Igrave	Contours detected: 3	Expected: 2
Glyph name: Iacute	Contours detected: 3	Expected: 2
Glyph name: Icircumflex	Contours detected: 3	Expected: 2
Glyph name: Idieresis	Contours detected: 4	Expected: 3
Glyph name: Eth	Contours detected: 3	Expected: 2
Glyph name: eth	Contours detected: 3	Expected: 2
Glyph name: yacute	Contours detected: 3	Expected: 2
Glyph name: thorn	Contours detected: 1	Expected: 2
Glyph name: ydieresis	Contours detected: 4	Expected: 3
Glyph name: aogonek	Contours detected: 3	Expected: 2
Glyph name: Dcroat	Contours detected: 3	Expected: 2
Glyph name: dcroat	Contours detected: 3	Expected: 2
Glyph name: eogonek	Contours detected: 3	Expected: 2
Glyph name: Itilde	Contours detected: 3	Expected: 2
Glyph name: Imacron	Contours detected: 3	Expected: 2
Glyph name: Ibreve	Contours detected: 3	Expected: 2
Glyph name: Iogonek	Contours detected: 3	Expected: 1 or 2
Glyph name: Idotaccent	Contours detected: 3	Expected: 2
Glyph name: Tbar	Contours detected: 2	Expected: 1
Glyph name: Uogonek	Contours detected: 2	Expected: 1
Glyph name: uogonek	Contours detected: 2	Expected: 1
Glyph name: ycircumflex	Contours detected: 3	Expected: 2
Glyph name: ohorn	Contours detected: 3	Expected: 2
Glyph name: Uhorn	Contours detected: 2	Expected: 1
Glyph name: uhorn	Contours detected: 2	Expected: 1
Glyph name: uni01EA	Contours detected: 3	Expected: 2
Glyph name: uni01EB	Contours detected: 3	Expected: 2
Glyph name: uni0203	Contours detected: 4	Expected: 3
Glyph name: uni0207	Contours detected: 4	Expected: 3
Glyph name: uni0208	Contours detected: 4	Expected: 3
Glyph name: uni020A	Contours detected: 3	Expected: 2
Glyph name: uni020F	Contours detected: 4	Expected: 3
Glyph name: uni0213	Contours detected: 3	Expected: 2
Glyph name: uni0217	Contours detected: 3	Expected: 2
Glyph name: uni0233	Contours detected: 3	Expected: 2
Glyph name: uni0311	Contours detected: 2	Expected: 1
Glyph name: uni1EC8	Contours detected: 3	Expected: 2
Glyph name: uni1ECA	Contours detected: 3	Expected: 2
Glyph name: uni1EDB	Contours detected: 4	Expected: 3
Glyph name: uni1EDD	Contours detected: 4	Expected: 3
Glyph name: uni1EDF	Contours detected: 4	Expected: 3
Glyph name: uni1EE1	Contours detected: 4	Expected: 3
Glyph name: uni1EE3	Contours detected: 4	Expected: 3
Glyph name: uni1EE8	Contours detected: 3	Expected: 2
Glyph name: uni1EE9	Contours detected: 3	Expected: 2
Glyph name: uni1EEA	Contours detected: 3	Expected: 2
Glyph name: uni1EEB	Contours detected: 3	Expected: 2
Glyph name: uni1EEC	Contours detected: 3	Expected: 2
Glyph name: uni1EED	Contours detected: 3	Expected: 2
Glyph name: uni1EEE	Contours detected: 3	Expected: 2
Glyph name: uni1EEF	Contours detected: 3	Expected: 2
Glyph name: uni1EF0	Contours detected: 3	Expected: 2
Glyph name: uni1EF1	Contours detected: 3	Expected: 2
Glyph name: ygrave	Contours detected: 3	Expected: 2
Glyph name: uni1EF5	Contours detected: 3	Expected: 2
Glyph name: uni1EF7	Contours detected: 3	Expected: 2
Glyph name: uni1EF9	Contours detected: 3	Expected: 2
Glyph name: uni20A6	Contours detected: 2	Expected: 1, 3 or 5
Glyph name: uni20A9	Contours detected: 5	Expected: 1, 3, 4 or 7
Glyph name: uni20BA	Contours detected: 2	Expected: 1
Glyph name: Dcroat	Contours detected: 3	Expected: 2
Glyph name: Eth	Contours detected: 3	Expected: 2
Glyph name: I	Contours detected: 2	Expected: 1
Glyph name: Iacute	Contours detected: 3	Expected: 2
Glyph name: Ibreve	Contours detected: 3	Expected: 2
Glyph name: Icircumflex	Contours detected: 3	Expected: 2
Glyph name: Idieresis	Contours detected: 4	Expected: 3
Glyph name: Idotaccent	Contours detected: 3	Expected: 2
Glyph name: Igrave	Contours detected: 3	Expected: 2
Glyph name: Imacron	Contours detected: 3	Expected: 2
Glyph name: Iogonek	Contours detected: 3	Expected: 1 or 2
Glyph name: Itilde	Contours detected: 3	Expected: 2
Glyph name: Tbar	Contours detected: 2	Expected: 1
Glyph name: Uhorn	Contours detected: 2	Expected: 1
Glyph name: Uogonek	Contours detected: 2	Expected: 1
Glyph name: aogonek	Contours detected: 3	Expected: 2
Glyph name: at	Contours detected: 1	Expected: 2
Glyph name: dcroat	Contours detected: 3	Expected: 2
Glyph name: eogonek	Contours detected: 3	Expected: 2
Glyph name: eth	Contours detected: 3	Expected: 2
Glyph name: ohorn	Contours detected: 3	Expected: 2
Glyph name: one	Contours detected: 2	Expected: 1
Glyph name: onehalf	Contours detected: 4	Expected: 3
Glyph name: thorn	Contours detected: 1	Expected: 2
Glyph name: uhorn	Contours detected: 2	Expected: 1
Glyph name: uni0233	Contours detected: 3	Expected: 2
Glyph name: uni0311	Contours detected: 2	Expected: 1
Glyph name: uni1EC8	Contours detected: 3	Expected: 2
Glyph name: uni1ECA	Contours detected: 3	Expected: 2
Glyph name: uni1EDB	Contours detected: 4	Expected: 3
Glyph name: uni1EDD	Contours detected: 4	Expected: 3
Glyph name: uni1EDF	Contours detected: 4	Expected: 3
Glyph name: uni1EE1	Contours detected: 4	Expected: 3
Glyph name: uni1EE3	Contours detected: 4	Expected: 3
Glyph name: uni1EE8	Contours detected: 3	Expected: 2
Glyph name: uni1EE9	Contours detected: 3	Expected: 2
Glyph name: uni1EEA	Contours detected: 3	Expected: 2
Glyph name: uni1EEB	Contours detected: 3	Expected: 2
Glyph name: uni1EEC	Contours detected: 3	Expected: 2
Glyph name: uni1EED	Contours detected: 3	Expected: 2
Glyph name: uni1EEE	Contours detected: 3	Expected: 2
Glyph name: uni1EEF	Contours detected: 3	Expected: 2
Glyph name: uni1EF0	Contours detected: 3	Expected: 2
Glyph name: uni1EF1	Contours detected: 3	Expected: 2
Glyph name: uni1EF5	Contours detected: 3	Expected: 2
Glyph name: uni1EF7	Contours detected: 3	Expected: 2
Glyph name: uni1EF9	Contours detected: 3	Expected: 2
Glyph name: uni20A6	Contours detected: 2	Expected: 1, 3 or 5
Glyph name: uni20A9	Contours detected: 5	Expected: 1, 3, 4 or 7
Glyph name: uni20BA	Contours detected: 2	Expected: 1
Glyph name: uogonek	Contours detected: 2	Expected: 1
Glyph name: y	Contours detected: 2	Expected: 1
Glyph name: yacute	Contours detected: 3	Expected: 2
Glyph name: ycircumflex	Contours detected: 3	Expected: 2
Glyph name: ydieresis	Contours detected: 4	Expected: 3
Glyph name: ygrave	Contours detected: 3	Expected: 2 [code: contour-count]

</details>
<details>
<summary>⚠ <b>WARN:</b> Are there caret positions declared for every ligature?</summary>

* [com.google.fonts/check/ligature_carets](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/ligature_carets)
<pre>--- Rationale ---
All ligatures in a font must have corresponding caret (text cursor) positions
defined in the GDEF table, otherwhise, users may experience issues with caret
rendering.
If using GlyphsApp or UFOs, ligature carets can be defined as anchors with names
starting with &#x27;caret_&#x27;. These can be compiled with fontmake as of version
v2.4.0.</pre>

* ⚠ **WARN** This font lacks caret position values for ligature glyphs on its GDEF table. [code: lacks-caret-pos]

</details>
<details>
<summary>⚠ <b>WARN:</b> Is there kerning info for non-ligated sequences?</summary>

* [com.google.fonts/check/kerning_for_non_ligated_sequences](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/kerning_for_non_ligated_sequences)
<pre>--- Rationale ---
Fonts with ligatures should have kerning on the corresponding non-ligated
sequences for text where ligatures aren&#x27;t used (eg
https://github.com/impallari/Raleway/issues/14).</pre>

* ⚠ **WARN** GPOS table lacks kerning info for the following non-ligated sequences:
	- f + f
	- f + i
	- i + f
	- f + l
	- l + f
	- i + l

   [code: lacks-kern-info]

</details>
<details>
<summary>⚠ <b>WARN:</b> Combined length of family and style must not exceed 27 characters.</summary>

* [com.google.fonts/check/name/family_and_style_max_length](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/name/family_and_style_max_length)
<pre>--- Rationale ---
According to a GlyphsApp tutorial [1], in order to make sure all versions of
Windows recognize it as a valid font file, we must make sure that the
concatenated length of the familyname (NameID.FONT_FAMILY_NAME) and style
(NameID.FONT_SUBFAMILY_NAME) strings in the name table do not exceed 20
characters.
After discussing the problem in more detail at `FontBakery issue #2179 [2] we
decided that allowing up to 27 chars would still be on the safe side, though.
[1] https://glyphsapp.com/tutorials/multiple-masters-part-3-setting-up-instances
[2] https://github.com/googlefonts/fontbakery/issues/2179</pre>

* ⚠ **WARN** The combined length of family and style exceeds 27 chars in the following 'WINDOWS' entries:
 FONT_FAMILY_NAME = 'Foldit Fallback[Expanded,ExtraBold]' / SUBFAMILY_NAME = 'Regular'

Please take a look at the conversation at https://github.com/googlefonts/fontbakery/issues/2179 in order to understand the reasoning behind these name table records max-length criteria. [code: too-long]

</details>
<details>
<summary>⚠ <b>WARN:</b> Ensure fonts have ScriptLangTags declared on the 'meta' table.</summary>

* [com.google.fonts/check/meta/script_lang_tags](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/meta/script_lang_tags)
<pre>--- Rationale ---
The OpenType &#x27;meta&#x27; table originated at Apple. Microsoft added it to OT with
just two DataMap records:
- dlng: comma-separated ScriptLangTags that indicate which scripts, or languages
and scripts, with possible variants, the font is designed for
- slng: comma-separated ScriptLangTags that indicate which scripts, or languages
and scripts, with possible variants, the font supports
The slng structure is intended to describe which languages and scripts the font
overall supports. For example, a Traditional Chinese font that also contains
Latin characters, can indicate Hant,Latn, showing that it supports Hant, the
Traditional Chinese variant of the Hani script, and it also supports the Latn
script
The dlng structure is far more interesting. A font may contain various glyphs,
but only a particular subset of the glyphs may be truly &quot;leading&quot; in the design,
while other glyphs may have been included for technical reasons. Such a
Traditional Chinese font could only list Hant there, showing that it’s designed
for Traditional Chinese, but the font would omit Latn, because the developers
don’t think the font is really recommended for purely Latin-script use.
The tags used in the structures can comprise just script, or also language and
script. For example, if a font has Bulgarian Cyrillic alternates in the locl
feature for the cyrl BGR OT languagesystem, it could also indicate in dlng
explicitly that it supports bul-Cyrl. (Note that the scripts and languages in
meta use the ISO language and script codes, not the OpenType ones).
This check ensures that the font has the meta table containing the slng and dlng
structures.
All families in the Google Fonts collection should contain the &#x27;meta&#x27; table.
Windows 10 already uses it when deciding on which fonts to fall back to. The
Google Fonts API and also other environments could use the data for smarter
filtering. Most importantly, those entries should be added to the Noto fonts.
In the font making process, some environments store this data in external files
already. But the meta table provides a convenient way to store this inside the
font file, so some tools may add the data, and unrelated tools may read this
data. This makes the solution much more portable and universal.</pre>

* ⚠ **WARN** This font file does not have a 'meta' table. [code: lacks-meta-table]

</details>
<details>
<summary>⚠ <b>WARN:</b> Do outlines contain any jaggy segments?</summary>

* [com.google.fonts/check/outline_jaggy_segments](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_jaggy_segments)
<pre>--- Rationale ---
This check heuristically detects outline segments which form a particularly
small angle, indicative of an outline error. This may cause false positives in
cases such as extreme ink traps, so should be regarded as advisory and backed up
by manual inspection.</pre>

* ⚠ **WARN** The following glyphs have jaggy segments:
	* asterisk (U+002A): L<<265.0,442.0>--<251.0,351.0>>/L<<251.0,351.0>--<311.0,730.0>> = 0.24975216281029114
	* d (U+0064): L<<782.0,329.0>--<780.0,331.0>>/L<<780.0,331.0>--<783.0,327.0>> = 8.13010235415596
	* dcaron (U+010F): L<<782.0,329.0>--<780.0,331.0>>/L<<780.0,331.0>--<783.0,327.0>> = 8.13010235415596
	* dcroat (U+0111): L<<782.0,329.0>--<780.0,331.0>>/L<<780.0,331.0>--<783.0,327.0>> = 8.13010235415596
	* dong (U+20AB): L<<782.0,377.0>--<780.0,379.0>>/L<<780.0,379.0>--<783.0,375.0>> = 8.13010235415596
	* eth (U+00F0): L<<782.0,329.0>--<781.0,330.0>>/L<<781.0,330.0>--<783.0,327.0>> = 11.309932474020227
	* kgreenlandic (U+0138): L<<248.0,794.0>--<249.0,400.0>>/L<<249.0,400.0>--<249.0,437.0>> = 0.1454204479278869
	* p (U+0070): L<<36.0,201.0>--<38.0,199.0>>/L<<38.0,199.0>--<35.0,203.0>> = 8.13010235415596
	* thorn (U+00FE): L<<36.0,201.0>--<38.0,199.0>>/L<<38.0,199.0>--<35.0,203.0>> = 8.13010235415596
	* uni01C6 (U+01C6): L<<782.0,329.0>--<780.0,331.0>>/L<<780.0,331.0>--<783.0,327.0>> = 8.13010235415596
	* uni20BA (U+20BA): L<<-109.0,455.0>--<-112.0,425.0>>/L<<-112.0,425.0>--<-112.0,576.0>> = 5.710593137499633 and uni20BA (U+20BA): L<<593.0,565.0>--<593.0,496.0>>/L<<593.0,496.0>--<592.0,565.0>> = 0.8303154862578446 [code: found-jaggy-segments]

</details>
<details>
<summary>⚠ <b>WARN:</b> Do outlines contain any semi-vertical or semi-horizontal lines?</summary>

* [com.google.fonts/check/outline_semi_vertical](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/<Section: Outline Correctness Checks>.html#com.google.fonts/check/outline_semi_vertical)
<pre>--- Rationale ---
This check detects line segments which are nearly, but not quite, exactly
horizontal or vertical. Sometimes such lines are created by design, but often
they are indicative of a design error.
This check is disabled for italic styles, which often contain nearly-upright
lines.</pre>

* ⚠ **WARN** The following glyphs have semi-vertical/semi-horizontal lines:
 * Euro (U+20AC): L<<344.0,333.0>--<824.0,334.0>>
 * Euro (U+20AC): L<<344.0,422.0>--<824.0,423.0>>
 * Euro (U+20AC): L<<847.0,310.0>--<344.0,309.0>>
 * Euro (U+20AC): L<<847.0,399.0>--<344.0,398.0>>
 * I (U+0049): L<<245.0,0.0>--<246.0,486.0>>
 * I (U+0049): L<<245.0,0.0>--<25.0,1.0>>
 * Iacute (U+00CD): L<<245.0,0.0>--<246.0,486.0>>
 * Iacute (U+00CD): L<<245.0,0.0>--<25.0,1.0>>
 * Ibreve (U+012C): L<<245.0,0.0>--<246.0,486.0>>
 * Ibreve (U+012C): L<<245.0,0.0>--<25.0,1.0>> and 91 more. [code: found-semi-vertical]

</details>
<br>
</details>

### Summary

| 💔 ERROR | 🔥 FAIL | ⚠ WARN | 💤 SKIP | ℹ INFO | 🍞 PASS | 🔎 DEBUG |
|:-----:|:----:|:----:|:----:|:----:|:----:|:----:|
| 24 | 24 | 38 | 425 | 29 | 284 | 0 |
| 3% | 3% | 5% | 52% | 4% | 34% | 0% |

**Note:** The following loglevels were omitted in this report:
* **SKIP**
* **INFO**
* **PASS**
* **DEBUG**
