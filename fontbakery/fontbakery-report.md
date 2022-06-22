## Fontbakery report

Fontbakery version: 0.8.2

<details>
<summary><b>[1] Family checks</b></summary>
<details>
<summary>🔥 <b>FAIL:</b> Checking all files are in the same directory.</summary>

* [com.google.fonts/check/family/single_directory](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/universal.html#com.google.fonts/check/family/single_directory)
<pre>--- Rationale ---
If the set of font files passed in the command line is not all in the same
directory, then we warn the user since the tool will interpret the set of files
as belonging to a single family (and it is unlikely that the user would store
the files from a single family spreaded in several separate directories).</pre>

* 🔥 **FAIL** Not all fonts passed in the command line are in the same directory. This may lead to bad results as the tool will interpret all font files as belonging to a single font family. The detected directories are: ['fonts/variable', 'fonts/ttf'] [code: single-directory]

</details>
<br>
</details>
<details>
<summary><b>[12] Foldit-decomposed[wght].ttf</b></summary>
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

* 🔥 **FAIL** The file 'Foldit-decomposed[wght].ttf' must be renamed to 'Foldit[wght].ttf' according to the Google Fonts naming policy for variable fonts. [code: bad-varfont-filename]

</details>
<details>
<summary>🔥 <b>FAIL:</b> Ensure variable fonts include an avar table.</summary>

* [com.google.fonts/check/mandatory_avar_table](https://font-bakery.readthedocs.io/en/latest/fontbakery/profiles/googlefonts.html#com.google.fonts/check/mandatory_avar_table)
<pre>--- Rationale ---
Most variable fonts should include an avar table to correctly define axes
progression rates.
For example, a weight axis from 0% to 100% doesn&#x27;t map directly to 100 to 1000,
because a 10% progression from 0% may be too much to define the 200, while 90%
may be too little to define the 900.
If the progression rates of axes is linear, this check can be ignored. Fontmake
will also skip adding an avar table if the progression rates are linear.
However, we still recommend designers visually proof each instance is at the
desired weight, width etc.</pre>

* 🔥 **FAIL** This variable font does not have an avar table. [code: missing-avar]

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
<br>
</details>
<details>
<summary><b>[15] Foldit-Thin.ttf</b></summary>
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
Glyph name: at	Contours detected: 1	Expected: 2 [code: contour-count]

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
	* Ibreve (U+012C): L<<193.0,839.0>--<162.0,803.0>> -> L<<162.0,803.0>--<143.0,781.0>>
	* Ibreve (U+012C): L<<87.0,781.0>--<68.0,803.0>> -> L<<68.0,803.0>--<37.0,839.0>>
	* Lcaron (U+013D): L<<151.0,700.0>--<151.0,699.0>> -> L<<151.0,699.0>--<146.0,570.0>>
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
	* V (U+0056): L<<47.0,700.0>--<119.0,103.0>>/L<<119.0,103.0>--<183.0,700.0>> = 12.995722982421416
	* colonmonetary (U+20A1): L<<82.0,676.0>--<82.0,272.0>>/L<<82.0,272.0>--<118.0,676.0>> = 5.0921151244989575
	* oslash (U+00F8): L<<124.0,24.0>--<124.0,298.0>>/L<<124.0,298.0>--<74.0,79.0>> = 12.860793059094537
	* oslash (U+00F8): L<<74.0,476.0>--<74.0,180.0>>/L<<74.0,180.0>--<124.0,399.0>> = 12.860793059094537
	* oslashacute (U+01FF): L<<124.0,24.0>--<124.0,298.0>>/L<<124.0,298.0>--<74.0,79.0>> = 12.860793059094537
	* oslashacute (U+01FF): L<<74.0,476.0>--<74.0,180.0>>/L<<74.0,180.0>--<124.0,399.0>> = 12.860793059094537
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
 * g (U+0067): L<<147.0,476.0>--<146.0,-177.0>>
 * gbreve (U+011F): L<<147.0,476.0>--<146.0,-177.0>>
 * gcaron (U+01E7): L<<147.0,476.0>--<146.0,-177.0>>
 * gcircumflex (U+011D): L<<147.0,476.0>--<146.0,-177.0>>
 * gdotaccent (U+0121): L<<147.0,476.0>--<146.0,-177.0>> and 18 more. [code: found-semi-vertical]

</details>
<br>
</details>
<details>
<summary><b>[14] Foldit-SemiBold.ttf</b></summary>
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
Glyph name: A	Contours detected: 1	Expected: 2
Glyph name: I	Contours detected: 2	Expected: 1
Glyph name: b	Contours detected: 1	Expected: 2
Glyph name: y	Contours detected: 2	Expected: 1
Glyph name: uni00B9	Contours detected: 2	Expected: 1
Glyph name: onehalf	Contours detected: 4	Expected: 3
Glyph name: Agrave	Contours detected: 2	Expected: 3
Glyph name: Aacute	Contours detected: 2	Expected: 3
Glyph name: Acircumflex	Contours detected: 2	Expected: 3
Glyph name: Atilde	Contours detected: 2	Expected: 3
Glyph name: Adieresis	Contours detected: 3	Expected: 4
Glyph name: Igrave	Contours detected: 3	Expected: 2
Glyph name: Iacute	Contours detected: 3	Expected: 2
Glyph name: Icircumflex	Contours detected: 3	Expected: 2
Glyph name: Idieresis	Contours detected: 4	Expected: 3
Glyph name: yacute	Contours detected: 3	Expected: 2
Glyph name: ydieresis	Contours detected: 4	Expected: 3
Glyph name: Amacron	Contours detected: 2	Expected: 3
Glyph name: Abreve	Contours detected: 2	Expected: 3
Glyph name: Aogonek	Contours detected: 1	Expected: 2 or 3
Glyph name: Itilde	Contours detected: 3	Expected: 2
Glyph name: Imacron	Contours detected: 3	Expected: 2
Glyph name: Ibreve	Contours detected: 3	Expected: 2
Glyph name: Idotaccent	Contours detected: 3	Expected: 2
Glyph name: ycircumflex	Contours detected: 3	Expected: 2
Glyph name: uni0200	Contours detected: 3	Expected: 4
Glyph name: uni0202	Contours detected: 2	Expected: 3
Glyph name: uni0208	Contours detected: 4	Expected: 3
Glyph name: uni020A	Contours detected: 3	Expected: 2
Glyph name: uni0233	Contours detected: 3	Expected: 2
Glyph name: uni1EA0	Contours detected: 2	Expected: 3
Glyph name: uni1EA2	Contours detected: 2	Expected: 3
Glyph name: uni1EA4	Contours detected: 3	Expected: 4
Glyph name: uni1EA6	Contours detected: 3	Expected: 4
Glyph name: uni1EA8	Contours detected: 3	Expected: 4
Glyph name: uni1EAA	Contours detected: 3	Expected: 4
Glyph name: uni1EAC	Contours detected: 3	Expected: 4
Glyph name: uni1EAE	Contours detected: 3	Expected: 4
Glyph name: uni1EB0	Contours detected: 3	Expected: 4
Glyph name: uni1EB2	Contours detected: 3	Expected: 4
Glyph name: uni1EB4	Contours detected: 3	Expected: 4
Glyph name: uni1EB6	Contours detected: 3	Expected: 4
Glyph name: uni1EC8	Contours detected: 3	Expected: 2
Glyph name: uni1ECA	Contours detected: 3	Expected: 2
Glyph name: ygrave	Contours detected: 3	Expected: 2
Glyph name: uni1EF5	Contours detected: 3	Expected: 2
Glyph name: uni1EF7	Contours detected: 3	Expected: 2
Glyph name: uni1EF9	Contours detected: 3	Expected: 2
Glyph name: uni20A6	Contours detected: 4	Expected: 1, 3 or 5
Glyph name: uni20A9	Contours detected: 5	Expected: 1, 3, 4 or 7
Glyph name: A	Contours detected: 1	Expected: 2
Glyph name: Aacute	Contours detected: 2	Expected: 3
Glyph name: Abreve	Contours detected: 2	Expected: 3
Glyph name: Acircumflex	Contours detected: 2	Expected: 3
Glyph name: Adieresis	Contours detected: 3	Expected: 4
Glyph name: Agrave	Contours detected: 2	Expected: 3
Glyph name: Amacron	Contours detected: 2	Expected: 3
Glyph name: Aogonek	Contours detected: 1	Expected: 2 or 3
Glyph name: Atilde	Contours detected: 2	Expected: 3
Glyph name: I	Contours detected: 2	Expected: 1
Glyph name: Iacute	Contours detected: 3	Expected: 2
Glyph name: Ibreve	Contours detected: 3	Expected: 2
Glyph name: Icircumflex	Contours detected: 3	Expected: 2
Glyph name: Idieresis	Contours detected: 4	Expected: 3
Glyph name: Idotaccent	Contours detected: 3	Expected: 2
Glyph name: Igrave	Contours detected: 3	Expected: 2
Glyph name: Imacron	Contours detected: 3	Expected: 2
Glyph name: Itilde	Contours detected: 3	Expected: 2
Glyph name: at	Contours detected: 1	Expected: 2
Glyph name: b	Contours detected: 1	Expected: 2
Glyph name: one	Contours detected: 2	Expected: 1
Glyph name: onehalf	Contours detected: 4	Expected: 3
Glyph name: uni0233	Contours detected: 3	Expected: 2
Glyph name: uni1EA0	Contours detected: 2	Expected: 3
Glyph name: uni1EA2	Contours detected: 2	Expected: 3
Glyph name: uni1EA4	Contours detected: 3	Expected: 4
Glyph name: uni1EA6	Contours detected: 3	Expected: 4
Glyph name: uni1EA8	Contours detected: 3	Expected: 4
Glyph name: uni1EAA	Contours detected: 3	Expected: 4
Glyph name: uni1EAC	Contours detected: 3	Expected: 4
Glyph name: uni1EAE	Contours detected: 3	Expected: 4
Glyph name: uni1EB0	Contours detected: 3	Expected: 4
Glyph name: uni1EB2	Contours detected: 3	Expected: 4
Glyph name: uni1EB4	Contours detected: 3	Expected: 4
Glyph name: uni1EB6	Contours detected: 3	Expected: 4
Glyph name: uni1EC8	Contours detected: 3	Expected: 2
Glyph name: uni1ECA	Contours detected: 3	Expected: 2
Glyph name: uni1EF5	Contours detected: 3	Expected: 2
Glyph name: uni1EF7	Contours detected: 3	Expected: 2
Glyph name: uni1EF9	Contours detected: 3	Expected: 2
Glyph name: uni20A6	Contours detected: 4	Expected: 1, 3 or 5
Glyph name: uni20A9	Contours detected: 5	Expected: 1, 3, 4 or 7
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
	* Uring (U+016E): L<<441.0,734.0>--<441.0,734.0>>/L<<441.0,734.0>--<293.0,733.0>> = 0.38712775415102074
	* d (U+0064): L<<676.0,354.0>--<675.0,355.0>>/L<<675.0,355.0>--<677.0,352.0>> = 11.309932474020227
	* dcaron (U+010F): L<<676.0,354.0>--<675.0,355.0>>/L<<675.0,355.0>--<677.0,352.0>> = 11.309932474020227
	* dcroat (U+0111): L<<676.0,354.0>--<675.0,355.0>>/L<<675.0,355.0>--<677.0,352.0>> = 11.309932474020227
	* dong (U+20AB): L<<668.0,335.0>--<667.0,337.0>>/L<<667.0,337.0>--<669.0,334.0>> = 7.125016348901757
	* p (U+0070): L<<39.0,171.0>--<40.0,170.0>>/L<<40.0,170.0>--<38.0,173.0>> = 11.309932474020227
	* q (U+0071): L<<487.0,-200.0>--<486.0,79.0>>/L<<486.0,79.0>--<486.0,0.0>> = 0.205360337495141 and uni01C6 (U+01C6): L<<676.0,354.0>--<675.0,355.0>>/L<<675.0,355.0>--<677.0,352.0>> = 11.309932474020227 [code: found-jaggy-segments]

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
 * Aring (U+00C5): L<<448.0,734.0>--<301.0,733.0>>
 * I (U+0049): L<<221.0,0.0>--<24.0,1.0>>
 * I (U+0049): L<<222.0,174.0>--<221.0,0.0>>
 * Iacute (U+00CD): L<<221.0,0.0>--<24.0,1.0>>
 * Iacute (U+00CD): L<<222.0,174.0>--<221.0,0.0>>
 * Ibreve (U+012C): L<<221.0,0.0>--<24.0,1.0>>
 * Ibreve (U+012C): L<<222.0,174.0>--<221.0,0.0>>
 * Icircumflex (U+00CE): L<<221.0,0.0>--<24.0,1.0>>
 * Icircumflex (U+00CE): L<<222.0,174.0>--<221.0,0.0>>
 * Idieresis (U+00CF): L<<221.0,0.0>--<24.0,1.0>> and 99 more. [code: found-semi-vertical]

</details>
<br>
</details>
<details>
<summary><b>[14] Foldit-ExtraLight.ttf</b></summary>
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
Glyph name: A	Contours detected: 1	Expected: 2
Glyph name: I	Contours detected: 2	Expected: 1
Glyph name: b	Contours detected: 1	Expected: 2
Glyph name: q	Contours detected: 1	Expected: 2
Glyph name: y	Contours detected: 2	Expected: 1
Glyph name: uni00B9	Contours detected: 2	Expected: 1
Glyph name: onehalf	Contours detected: 4	Expected: 3
Glyph name: Agrave	Contours detected: 2	Expected: 3
Glyph name: Aacute	Contours detected: 2	Expected: 3
Glyph name: Acircumflex	Contours detected: 2	Expected: 3
Glyph name: Atilde	Contours detected: 2	Expected: 3
Glyph name: Adieresis	Contours detected: 3	Expected: 4
Glyph name: Igrave	Contours detected: 3	Expected: 2
Glyph name: Iacute	Contours detected: 3	Expected: 2
Glyph name: Icircumflex	Contours detected: 3	Expected: 2
Glyph name: Idieresis	Contours detected: 4	Expected: 3
Glyph name: yacute	Contours detected: 3	Expected: 2
Glyph name: ydieresis	Contours detected: 4	Expected: 3
Glyph name: Amacron	Contours detected: 2	Expected: 3
Glyph name: Abreve	Contours detected: 2	Expected: 3
Glyph name: Aogonek	Contours detected: 1	Expected: 2 or 3
Glyph name: Itilde	Contours detected: 3	Expected: 2
Glyph name: Imacron	Contours detected: 3	Expected: 2
Glyph name: Ibreve	Contours detected: 3	Expected: 2
Glyph name: Idotaccent	Contours detected: 3	Expected: 2
Glyph name: ycircumflex	Contours detected: 3	Expected: 2
Glyph name: uni0200	Contours detected: 3	Expected: 4
Glyph name: uni0202	Contours detected: 2	Expected: 3
Glyph name: uni0208	Contours detected: 4	Expected: 3
Glyph name: uni020A	Contours detected: 3	Expected: 2
Glyph name: uni0233	Contours detected: 3	Expected: 2
Glyph name: uni1EA0	Contours detected: 2	Expected: 3
Glyph name: uni1EA2	Contours detected: 2	Expected: 3
Glyph name: uni1EA4	Contours detected: 3	Expected: 4
Glyph name: uni1EA6	Contours detected: 3	Expected: 4
Glyph name: uni1EA8	Contours detected: 3	Expected: 4
Glyph name: uni1EAA	Contours detected: 3	Expected: 4
Glyph name: uni1EAC	Contours detected: 3	Expected: 4
Glyph name: uni1EAE	Contours detected: 3	Expected: 4
Glyph name: uni1EB0	Contours detected: 3	Expected: 4
Glyph name: uni1EB2	Contours detected: 3	Expected: 4
Glyph name: uni1EB4	Contours detected: 3	Expected: 4
Glyph name: uni1EB6	Contours detected: 3	Expected: 4
Glyph name: uni1EC8	Contours detected: 3	Expected: 2
Glyph name: uni1ECA	Contours detected: 3	Expected: 2
Glyph name: ygrave	Contours detected: 3	Expected: 2
Glyph name: uni1EF5	Contours detected: 3	Expected: 2
Glyph name: uni1EF7	Contours detected: 3	Expected: 2
Glyph name: uni1EF9	Contours detected: 3	Expected: 2
Glyph name: A	Contours detected: 1	Expected: 2
Glyph name: Aacute	Contours detected: 2	Expected: 3
Glyph name: Abreve	Contours detected: 2	Expected: 3
Glyph name: Acircumflex	Contours detected: 2	Expected: 3
Glyph name: Adieresis	Contours detected: 3	Expected: 4
Glyph name: Agrave	Contours detected: 2	Expected: 3
Glyph name: Amacron	Contours detected: 2	Expected: 3
Glyph name: Aogonek	Contours detected: 1	Expected: 2 or 3
Glyph name: Atilde	Contours detected: 2	Expected: 3
Glyph name: I	Contours detected: 2	Expected: 1
Glyph name: Iacute	Contours detected: 3	Expected: 2
Glyph name: Ibreve	Contours detected: 3	Expected: 2
Glyph name: Icircumflex	Contours detected: 3	Expected: 2
Glyph name: Idieresis	Contours detected: 4	Expected: 3
Glyph name: Idotaccent	Contours detected: 3	Expected: 2
Glyph name: Igrave	Contours detected: 3	Expected: 2
Glyph name: Imacron	Contours detected: 3	Expected: 2
Glyph name: Itilde	Contours detected: 3	Expected: 2
Glyph name: at	Contours detected: 1	Expected: 2
Glyph name: b	Contours detected: 1	Expected: 2
Glyph name: one	Contours detected: 2	Expected: 1
Glyph name: onehalf	Contours detected: 4	Expected: 3
Glyph name: q	Contours detected: 1	Expected: 2
Glyph name: uni0233	Contours detected: 3	Expected: 2
Glyph name: uni1EA0	Contours detected: 2	Expected: 3
Glyph name: uni1EA2	Contours detected: 2	Expected: 3
Glyph name: uni1EA4	Contours detected: 3	Expected: 4
Glyph name: uni1EA6	Contours detected: 3	Expected: 4
Glyph name: uni1EA8	Contours detected: 3	Expected: 4
Glyph name: uni1EAA	Contours detected: 3	Expected: 4
Glyph name: uni1EAC	Contours detected: 3	Expected: 4
Glyph name: uni1EAE	Contours detected: 3	Expected: 4
Glyph name: uni1EB0	Contours detected: 3	Expected: 4
Glyph name: uni1EB2	Contours detected: 3	Expected: 4
Glyph name: uni1EB4	Contours detected: 3	Expected: 4
Glyph name: uni1EB6	Contours detected: 3	Expected: 4
Glyph name: uni1EC8	Contours detected: 3	Expected: 2
Glyph name: uni1ECA	Contours detected: 3	Expected: 2
Glyph name: uni1EF5	Contours detected: 3	Expected: 2
Glyph name: uni1EF7	Contours detected: 3	Expected: 2
Glyph name: uni1EF9	Contours detected: 3	Expected: 2
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
	* colonmonetary (U+20A1): L<<108.0,651.0>--<108.0,92.0>>/L<<108.0,92.0>--<170.0,651.0>> = 6.328941838433589 [code: found-jaggy-segments]

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
 * Euro (U+20AC): L<<161.0,350.0>--<347.0,351.0>>
 * Euro (U+20AC): L<<161.0,439.0>--<347.0,440.0>>
 * Euro (U+20AC): L<<370.0,327.0>--<161.0,326.0>>
 * Euro (U+20AC): L<<370.0,416.0>--<161.0,415.0>>
 * M (U+004D): L<<482.0,689.0>--<480.0,0.0>>
 * dollar (U+0024): L<<200.0,651.0>--<201.0,392.0>>
 * g (U+0067): L<<247.0,451.0>--<246.0,-165.0>>
 * gbreve (U+011F): L<<247.0,451.0>--<246.0,-165.0>>
 * gcaron (U+01E7): L<<247.0,451.0>--<246.0,-165.0>>
 * gcircumflex (U+011D): L<<247.0,451.0>--<246.0,-165.0>> and 26 more. [code: found-semi-vertical]

</details>
<br>
</details>
<details>
<summary><b>[14] Foldit-Medium.ttf</b></summary>
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
Glyph name: A	Contours detected: 1	Expected: 2
Glyph name: I	Contours detected: 2	Expected: 1
Glyph name: b	Contours detected: 1	Expected: 2
Glyph name: q	Contours detected: 1	Expected: 2
Glyph name: y	Contours detected: 2	Expected: 1
Glyph name: uni00B9	Contours detected: 2	Expected: 1
Glyph name: onehalf	Contours detected: 4	Expected: 3
Glyph name: Agrave	Contours detected: 2	Expected: 3
Glyph name: Aacute	Contours detected: 2	Expected: 3
Glyph name: Acircumflex	Contours detected: 2	Expected: 3
Glyph name: Atilde	Contours detected: 2	Expected: 3
Glyph name: Adieresis	Contours detected: 3	Expected: 4
Glyph name: Igrave	Contours detected: 3	Expected: 2
Glyph name: Iacute	Contours detected: 3	Expected: 2
Glyph name: Icircumflex	Contours detected: 3	Expected: 2
Glyph name: Idieresis	Contours detected: 4	Expected: 3
Glyph name: yacute	Contours detected: 3	Expected: 2
Glyph name: ydieresis	Contours detected: 4	Expected: 3
Glyph name: Amacron	Contours detected: 2	Expected: 3
Glyph name: Abreve	Contours detected: 2	Expected: 3
Glyph name: Aogonek	Contours detected: 1	Expected: 2 or 3
Glyph name: Itilde	Contours detected: 3	Expected: 2
Glyph name: Imacron	Contours detected: 3	Expected: 2
Glyph name: Ibreve	Contours detected: 3	Expected: 2
Glyph name: Idotaccent	Contours detected: 3	Expected: 2
Glyph name: ycircumflex	Contours detected: 3	Expected: 2
Glyph name: uni0200	Contours detected: 3	Expected: 4
Glyph name: uni0202	Contours detected: 2	Expected: 3
Glyph name: uni0208	Contours detected: 4	Expected: 3
Glyph name: uni020A	Contours detected: 3	Expected: 2
Glyph name: uni0233	Contours detected: 3	Expected: 2
Glyph name: uni1EA0	Contours detected: 2	Expected: 3
Glyph name: uni1EA2	Contours detected: 2	Expected: 3
Glyph name: uni1EA4	Contours detected: 3	Expected: 4
Glyph name: uni1EA6	Contours detected: 3	Expected: 4
Glyph name: uni1EA8	Contours detected: 3	Expected: 4
Glyph name: uni1EAA	Contours detected: 3	Expected: 4
Glyph name: uni1EAC	Contours detected: 3	Expected: 4
Glyph name: uni1EAE	Contours detected: 3	Expected: 4
Glyph name: uni1EB0	Contours detected: 3	Expected: 4
Glyph name: uni1EB2	Contours detected: 3	Expected: 4
Glyph name: uni1EB4	Contours detected: 3	Expected: 4
Glyph name: uni1EB6	Contours detected: 3	Expected: 4
Glyph name: uni1EC8	Contours detected: 3	Expected: 2
Glyph name: uni1ECA	Contours detected: 3	Expected: 2
Glyph name: ygrave	Contours detected: 3	Expected: 2
Glyph name: uni1EF5	Contours detected: 3	Expected: 2
Glyph name: uni1EF7	Contours detected: 3	Expected: 2
Glyph name: uni1EF9	Contours detected: 3	Expected: 2
Glyph name: uni20A6	Contours detected: 4	Expected: 1, 3 or 5
Glyph name: uni20A9	Contours detected: 5	Expected: 1, 3, 4 or 7
Glyph name: A	Contours detected: 1	Expected: 2
Glyph name: Aacute	Contours detected: 2	Expected: 3
Glyph name: Abreve	Contours detected: 2	Expected: 3
Glyph name: Acircumflex	Contours detected: 2	Expected: 3
Glyph name: Adieresis	Contours detected: 3	Expected: 4
Glyph name: Agrave	Contours detected: 2	Expected: 3
Glyph name: Amacron	Contours detected: 2	Expected: 3
Glyph name: Aogonek	Contours detected: 1	Expected: 2 or 3
Glyph name: Atilde	Contours detected: 2	Expected: 3
Glyph name: I	Contours detected: 2	Expected: 1
Glyph name: Iacute	Contours detected: 3	Expected: 2
Glyph name: Ibreve	Contours detected: 3	Expected: 2
Glyph name: Icircumflex	Contours detected: 3	Expected: 2
Glyph name: Idieresis	Contours detected: 4	Expected: 3
Glyph name: Idotaccent	Contours detected: 3	Expected: 2
Glyph name: Igrave	Contours detected: 3	Expected: 2
Glyph name: Imacron	Contours detected: 3	Expected: 2
Glyph name: Itilde	Contours detected: 3	Expected: 2
Glyph name: at	Contours detected: 1	Expected: 2
Glyph name: b	Contours detected: 1	Expected: 2
Glyph name: one	Contours detected: 2	Expected: 1
Glyph name: onehalf	Contours detected: 4	Expected: 3
Glyph name: q	Contours detected: 1	Expected: 2
Glyph name: uni0233	Contours detected: 3	Expected: 2
Glyph name: uni1EA0	Contours detected: 2	Expected: 3
Glyph name: uni1EA2	Contours detected: 2	Expected: 3
Glyph name: uni1EA4	Contours detected: 3	Expected: 4
Glyph name: uni1EA6	Contours detected: 3	Expected: 4
Glyph name: uni1EA8	Contours detected: 3	Expected: 4
Glyph name: uni1EAA	Contours detected: 3	Expected: 4
Glyph name: uni1EAC	Contours detected: 3	Expected: 4
Glyph name: uni1EAE	Contours detected: 3	Expected: 4
Glyph name: uni1EB0	Contours detected: 3	Expected: 4
Glyph name: uni1EB2	Contours detected: 3	Expected: 4
Glyph name: uni1EB4	Contours detected: 3	Expected: 4
Glyph name: uni1EB6	Contours detected: 3	Expected: 4
Glyph name: uni1EC8	Contours detected: 3	Expected: 2
Glyph name: uni1ECA	Contours detected: 3	Expected: 2
Glyph name: uni1EF5	Contours detected: 3	Expected: 2
Glyph name: uni1EF7	Contours detected: 3	Expected: 2
Glyph name: uni1EF9	Contours detected: 3	Expected: 2
Glyph name: uni20A6	Contours detected: 4	Expected: 1, 3 or 5
Glyph name: uni20A9	Contours detected: 5	Expected: 1, 3, 4 or 7
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
	* Aring (U+00C5): L<<389.0,738.0>--<389.0,738.0>>/L<<389.0,738.0>--<263.0,737.0>> = 0.45471886169316617 and Uring (U+016E): L<<384.0,738.0>--<384.0,738.0>>/L<<384.0,738.0>--<258.0,737.0>> = 0.45471886169316617 [code: found-jaggy-segments]

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
 * A (U+0041): L<<464.0,351.0>--<465.0,576.0>>
 * Aacute (U+00C1): L<<464.0,351.0>--<465.0,576.0>>
 * Abreve (U+0102): L<<464.0,351.0>--<465.0,576.0>>
 * Acircumflex (U+00C2): L<<464.0,351.0>--<465.0,576.0>>
 * Adieresis (U+00C4): L<<464.0,351.0>--<465.0,576.0>>
 * Agrave (U+00C0): L<<464.0,351.0>--<465.0,576.0>>
 * Amacron (U+0100): L<<464.0,351.0>--<465.0,576.0>>
 * Aogonek (U+0104): L<<464.0,351.0>--<465.0,576.0>>
 * Aring (U+00C5): L<<389.0,738.0>--<263.0,737.0>>
 * Aring (U+00C5): L<<464.0,351.0>--<465.0,576.0>> and 112 more. [code: found-semi-vertical]

</details>
<br>
</details>
<details>
<summary><b>[15] Foldit-Bold.ttf</b></summary>
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
Glyph name: b	Contours detected: 1	Expected: 2
Glyph name: y	Contours detected: 2	Expected: 1
Glyph name: uni00B9	Contours detected: 2	Expected: 1
Glyph name: onehalf	Contours detected: 4	Expected: 3
Glyph name: Igrave	Contours detected: 3	Expected: 2
Glyph name: Iacute	Contours detected: 3	Expected: 2
Glyph name: Icircumflex	Contours detected: 3	Expected: 2
Glyph name: Idieresis	Contours detected: 4	Expected: 3
Glyph name: yacute	Contours detected: 3	Expected: 2
Glyph name: ydieresis	Contours detected: 4	Expected: 3
Glyph name: Itilde	Contours detected: 3	Expected: 2
Glyph name: Imacron	Contours detected: 3	Expected: 2
Glyph name: Ibreve	Contours detected: 3	Expected: 2
Glyph name: Idotaccent	Contours detected: 3	Expected: 2
Glyph name: ycircumflex	Contours detected: 3	Expected: 2
Glyph name: uni0208	Contours detected: 4	Expected: 3
Glyph name: uni020A	Contours detected: 3	Expected: 2
Glyph name: uni0233	Contours detected: 3	Expected: 2
Glyph name: uni1EC8	Contours detected: 3	Expected: 2
Glyph name: uni1ECA	Contours detected: 3	Expected: 2
Glyph name: ygrave	Contours detected: 3	Expected: 2
Glyph name: uni1EF5	Contours detected: 3	Expected: 2
Glyph name: uni1EF7	Contours detected: 3	Expected: 2
Glyph name: uni1EF9	Contours detected: 3	Expected: 2
Glyph name: uni20A9	Contours detected: 5	Expected: 1, 3, 4 or 7
Glyph name: I	Contours detected: 2	Expected: 1
Glyph name: Iacute	Contours detected: 3	Expected: 2
Glyph name: Ibreve	Contours detected: 3	Expected: 2
Glyph name: Icircumflex	Contours detected: 3	Expected: 2
Glyph name: Idieresis	Contours detected: 4	Expected: 3
Glyph name: Idotaccent	Contours detected: 3	Expected: 2
Glyph name: Igrave	Contours detected: 3	Expected: 2
Glyph name: Imacron	Contours detected: 3	Expected: 2
Glyph name: Itilde	Contours detected: 3	Expected: 2
Glyph name: at	Contours detected: 1	Expected: 2
Glyph name: b	Contours detected: 1	Expected: 2
Glyph name: one	Contours detected: 2	Expected: 1
Glyph name: onehalf	Contours detected: 4	Expected: 3
Glyph name: uni0233	Contours detected: 3	Expected: 2
Glyph name: uni1EC8	Contours detected: 3	Expected: 2
Glyph name: uni1ECA	Contours detected: 3	Expected: 2
Glyph name: uni1EF5	Contours detected: 3	Expected: 2
Glyph name: uni1EF7	Contours detected: 3	Expected: 2
Glyph name: uni1EF9	Contours detected: 3	Expected: 2
Glyph name: uni20A9	Contours detected: 5	Expected: 1, 3, 4 or 7
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
	* Abreve (U+0102): L<<314.0,760.0>--<220.0,860.0>> -> L<<220.0,860.0>--<186.0,898.0>>
	* Abreve (U+0102): L<<687.0,899.0>--<653.0,860.0>> -> L<<653.0,860.0>--<559.0,760.0>>
	* Ebreve (U+0114): L<<294.0,760.0>--<200.0,860.0>> -> L<<200.0,860.0>--<166.0,898.0>>
	* Ebreve (U+0114): L<<667.0,899.0>--<633.0,860.0>> -> L<<633.0,860.0>--<539.0,760.0>>
	* Gbreve (U+011E): L<<351.0,760.0>--<257.0,860.0>> -> L<<257.0,860.0>--<223.0,898.0>>
	* Gbreve (U+011E): L<<724.0,899.0>--<690.0,860.0>> -> L<<690.0,860.0>--<596.0,760.0>>
	* Ibreve (U+012C): L<<209.0,760.0>--<115.0,860.0>> -> L<<115.0,860.0>--<81.0,898.0>>
	* Ibreve (U+012C): L<<582.0,899.0>--<548.0,860.0>> -> L<<548.0,860.0>--<454.0,760.0>>
	* Obreve (U+014E): L<<304.0,760.0>--<210.0,860.0>> -> L<<210.0,860.0>--<176.0,898.0>>
	* Obreve (U+014E): L<<677.0,899.0>--<643.0,860.0>> -> L<<643.0,860.0>--<549.0,760.0>> and 86 more. [code: found-colinear-vectors]

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
	* Y (U+0059): L<<396.0,467.0>--<294.0,285.0>>/L<<294.0,285.0>--<546.0,730.0>> = 0.2545412189937722
	* Yacute (U+00DD): L<<396.0,467.0>--<294.0,285.0>>/L<<294.0,285.0>--<546.0,730.0>> = 0.2545412189937722
	* Ycircumflex (U+0176): L<<396.0,467.0>--<294.0,285.0>>/L<<294.0,285.0>--<546.0,730.0>> = 0.2545412189937722
	* Ydieresis (U+0178): L<<396.0,467.0>--<294.0,285.0>>/L<<294.0,285.0>--<546.0,730.0>> = 0.2545412189937722
	* Ygrave (U+1EF2): L<<396.0,467.0>--<294.0,285.0>>/L<<294.0,285.0>--<546.0,730.0>> = 0.2545412189937722
	* asterisk (U+002A): L<<225.0,442.0>--<211.0,351.0>>/L<<211.0,351.0>--<271.0,730.0>> = 0.24975216281029114
	* d (U+0064): L<<782.0,329.0>--<780.0,331.0>>/L<<780.0,331.0>--<783.0,327.0>> = 8.13010235415596
	* dcaron (U+010F): L<<782.0,329.0>--<780.0,331.0>>/L<<780.0,331.0>--<783.0,327.0>> = 8.13010235415596
	* dcroat (U+0111): L<<782.0,329.0>--<780.0,331.0>>/L<<780.0,331.0>--<783.0,327.0>> = 8.13010235415596
	* dong (U+20AB): L<<772.0,307.0>--<770.0,309.0>>/L<<770.0,309.0>--<773.0,305.0>> = 8.13010235415596 and 8 more. [code: found-jaggy-segments]

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
 * Euro (U+20AC): L<<304.0,333.0>--<824.0,334.0>>
 * Euro (U+20AC): L<<304.0,422.0>--<824.0,423.0>>
 * Euro (U+20AC): L<<847.0,310.0>--<304.0,309.0>>
 * Euro (U+20AC): L<<847.0,399.0>--<304.0,398.0>>
 * I (U+0049): L<<245.0,0.0>--<25.0,1.0>>
 * I (U+0049): L<<246.0,204.0>--<245.0,0.0>>
 * Iacute (U+00CD): L<<245.0,0.0>--<25.0,1.0>>
 * Iacute (U+00CD): L<<246.0,204.0>--<245.0,0.0>>
 * Ibreve (U+012C): L<<245.0,0.0>--<25.0,1.0>>
 * Ibreve (U+012C): L<<246.0,204.0>--<245.0,0.0>> and 91 more. [code: found-semi-vertical]

</details>
<br>
</details>
<details>
<summary><b>[14] Foldit-Black.ttf</b></summary>
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
Glyph name: b	Contours detected: 1	Expected: 2
Glyph name: uni00B9	Contours detected: 2	Expected: 1
Glyph name: onehalf	Contours detected: 4	Expected: 3
Glyph name: uni20A6	Contours detected: 2	Expected: 1, 3 or 5
Glyph name: uni20A9	Contours detected: 5	Expected: 1, 3, 4 or 7
Glyph name: b	Contours detected: 1	Expected: 2
Glyph name: one	Contours detected: 2	Expected: 1
Glyph name: onehalf	Contours detected: 4	Expected: 3
Glyph name: uni20A6	Contours detected: 2	Expected: 1, 3 or 5
Glyph name: uni20A9	Contours detected: 5	Expected: 1, 3, 4 or 7 [code: contour-count]

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
	* asterisk (U+002A): L<<225.0,442.0>--<211.0,351.0>>/L<<211.0,351.0>--<271.0,730.0>> = 0.24975216281029114
	* d (U+0064): L<<862.0,289.0>--<861.0,290.0>>/L<<861.0,290.0>--<863.0,287.0>> = 11.309932474020227
	* dcaron (U+010F): L<<862.0,289.0>--<861.0,290.0>>/L<<861.0,290.0>--<863.0,287.0>> = 11.309932474020227
	* dcroat (U+0111): L<<862.0,289.0>--<861.0,290.0>>/L<<861.0,290.0>--<863.0,287.0>> = 11.309932474020227
	* dong (U+20AB): L<<852.0,319.0>--<849.0,322.0>>/L<<849.0,322.0>--<853.0,317.0>> = 6.3401917459097925
	* oe (U+0153): L<<1201.0,221.0>--<842.0,220.0>>/L<<842.0,220.0>--<842.0,220.0>> = 0.15959785884710373
	* p (U+0070): L<<36.0,241.0>--<39.0,238.0>>/L<<39.0,238.0>--<35.0,243.0>> = 6.340191745909908 and uni01C6 (U+01C6): L<<862.0,289.0>--<861.0,290.0>>/L<<861.0,290.0>--<863.0,287.0>> = 11.309932474020227 [code: found-jaggy-segments]

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
 * G (U+0047): L<<299.0,466.0>--<728.0,467.0>>
 * Gbreve (U+011E): L<<299.0,466.0>--<728.0,467.0>>
 * Gcaron (U+01E6): L<<299.0,466.0>--<728.0,467.0>>
 * Gcircumflex (U+011C): L<<299.0,466.0>--<728.0,467.0>>
 * Gdotaccent (U+0120): L<<299.0,466.0>--<728.0,467.0>>
 * I (U+0049): L<<246.0,0.0>--<25.0,1.0>> and 81 more. [code: found-semi-vertical]

</details>
<br>
</details>
<details>
<summary><b>[14] Foldit-Regular.ttf</b></summary>
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
Glyph name: A	Contours detected: 1	Expected: 2
Glyph name: I	Contours detected: 2	Expected: 1
Glyph name: b	Contours detected: 1	Expected: 2
Glyph name: q	Contours detected: 1	Expected: 2
Glyph name: y	Contours detected: 2	Expected: 1
Glyph name: uni00B9	Contours detected: 2	Expected: 1
Glyph name: onehalf	Contours detected: 4	Expected: 3
Glyph name: Agrave	Contours detected: 2	Expected: 3
Glyph name: Aacute	Contours detected: 2	Expected: 3
Glyph name: Acircumflex	Contours detected: 2	Expected: 3
Glyph name: Atilde	Contours detected: 2	Expected: 3
Glyph name: Adieresis	Contours detected: 3	Expected: 4
Glyph name: Igrave	Contours detected: 3	Expected: 2
Glyph name: Iacute	Contours detected: 3	Expected: 2
Glyph name: Icircumflex	Contours detected: 3	Expected: 2
Glyph name: Idieresis	Contours detected: 4	Expected: 3
Glyph name: yacute	Contours detected: 3	Expected: 2
Glyph name: thorn	Contours detected: 3	Expected: 2
Glyph name: ydieresis	Contours detected: 4	Expected: 3
Glyph name: Amacron	Contours detected: 2	Expected: 3
Glyph name: Abreve	Contours detected: 2	Expected: 3
Glyph name: Aogonek	Contours detected: 1	Expected: 2 or 3
Glyph name: Itilde	Contours detected: 3	Expected: 2
Glyph name: Imacron	Contours detected: 3	Expected: 2
Glyph name: Ibreve	Contours detected: 3	Expected: 2
Glyph name: Idotaccent	Contours detected: 3	Expected: 2
Glyph name: ycircumflex	Contours detected: 3	Expected: 2
Glyph name: uni0200	Contours detected: 3	Expected: 4
Glyph name: uni0202	Contours detected: 2	Expected: 3
Glyph name: uni0208	Contours detected: 4	Expected: 3
Glyph name: uni020A	Contours detected: 3	Expected: 2
Glyph name: uni0233	Contours detected: 3	Expected: 2
Glyph name: uni1EA0	Contours detected: 2	Expected: 3
Glyph name: uni1EA2	Contours detected: 2	Expected: 3
Glyph name: uni1EA4	Contours detected: 3	Expected: 4
Glyph name: uni1EA6	Contours detected: 3	Expected: 4
Glyph name: uni1EA8	Contours detected: 3	Expected: 4
Glyph name: uni1EAA	Contours detected: 3	Expected: 4
Glyph name: uni1EAC	Contours detected: 3	Expected: 4
Glyph name: uni1EAE	Contours detected: 3	Expected: 4
Glyph name: uni1EB0	Contours detected: 3	Expected: 4
Glyph name: uni1EB2	Contours detected: 3	Expected: 4
Glyph name: uni1EB4	Contours detected: 3	Expected: 4
Glyph name: uni1EB6	Contours detected: 3	Expected: 4
Glyph name: uni1EC8	Contours detected: 3	Expected: 2
Glyph name: uni1ECA	Contours detected: 3	Expected: 2
Glyph name: ygrave	Contours detected: 3	Expected: 2
Glyph name: uni1EF5	Contours detected: 3	Expected: 2
Glyph name: uni1EF7	Contours detected: 3	Expected: 2
Glyph name: uni1EF9	Contours detected: 3	Expected: 2
Glyph name: uni20A6	Contours detected: 4	Expected: 1, 3 or 5
Glyph name: uni20A9	Contours detected: 5	Expected: 1, 3, 4 or 7
Glyph name: A	Contours detected: 1	Expected: 2
Glyph name: Aacute	Contours detected: 2	Expected: 3
Glyph name: Abreve	Contours detected: 2	Expected: 3
Glyph name: Acircumflex	Contours detected: 2	Expected: 3
Glyph name: Adieresis	Contours detected: 3	Expected: 4
Glyph name: Agrave	Contours detected: 2	Expected: 3
Glyph name: Amacron	Contours detected: 2	Expected: 3
Glyph name: Aogonek	Contours detected: 1	Expected: 2 or 3
Glyph name: Atilde	Contours detected: 2	Expected: 3
Glyph name: I	Contours detected: 2	Expected: 1
Glyph name: Iacute	Contours detected: 3	Expected: 2
Glyph name: Ibreve	Contours detected: 3	Expected: 2
Glyph name: Icircumflex	Contours detected: 3	Expected: 2
Glyph name: Idieresis	Contours detected: 4	Expected: 3
Glyph name: Idotaccent	Contours detected: 3	Expected: 2
Glyph name: Igrave	Contours detected: 3	Expected: 2
Glyph name: Imacron	Contours detected: 3	Expected: 2
Glyph name: Itilde	Contours detected: 3	Expected: 2
Glyph name: at	Contours detected: 1	Expected: 2
Glyph name: b	Contours detected: 1	Expected: 2
Glyph name: one	Contours detected: 2	Expected: 1
Glyph name: onehalf	Contours detected: 4	Expected: 3
Glyph name: q	Contours detected: 1	Expected: 2
Glyph name: thorn	Contours detected: 3	Expected: 2
Glyph name: uni0233	Contours detected: 3	Expected: 2
Glyph name: uni1EA0	Contours detected: 2	Expected: 3
Glyph name: uni1EA2	Contours detected: 2	Expected: 3
Glyph name: uni1EA4	Contours detected: 3	Expected: 4
Glyph name: uni1EA6	Contours detected: 3	Expected: 4
Glyph name: uni1EA8	Contours detected: 3	Expected: 4
Glyph name: uni1EAA	Contours detected: 3	Expected: 4
Glyph name: uni1EAC	Contours detected: 3	Expected: 4
Glyph name: uni1EAE	Contours detected: 3	Expected: 4
Glyph name: uni1EB0	Contours detected: 3	Expected: 4
Glyph name: uni1EB2	Contours detected: 3	Expected: 4
Glyph name: uni1EB4	Contours detected: 3	Expected: 4
Glyph name: uni1EB6	Contours detected: 3	Expected: 4
Glyph name: uni1EC8	Contours detected: 3	Expected: 2
Glyph name: uni1ECA	Contours detected: 3	Expected: 2
Glyph name: uni1EF5	Contours detected: 3	Expected: 2
Glyph name: uni1EF7	Contours detected: 3	Expected: 2
Glyph name: uni1EF9	Contours detected: 3	Expected: 2
Glyph name: uni20A6	Contours detected: 4	Expected: 1, 3 or 5
Glyph name: uni20A9	Contours detected: 5	Expected: 1, 3, 4 or 7
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
	* section (U+00A7): L<<181.0,498.0>--<197.0,487.0>>/L<<197.0,487.0>--<75.0,616.0>> = 12.08895320957726 [code: found-jaggy-segments]

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
 * A (U+0041): L<<397.0,263.0>--<398.0,601.0>>
 * A (U+0041): L<<398.0,0.0>--<397.0,263.0>>
 * Aacute (U+00C1): L<<397.0,263.0>--<398.0,601.0>>
 * Aacute (U+00C1): L<<398.0,0.0>--<397.0,263.0>>
 * Abreve (U+0102): L<<397.0,263.0>--<398.0,601.0>>
 * Abreve (U+0102): L<<398.0,0.0>--<397.0,263.0>>
 * Acircumflex (U+00C2): L<<397.0,263.0>--<398.0,601.0>>
 * Acircumflex (U+00C2): L<<398.0,0.0>--<397.0,263.0>>
 * Adieresis (U+00C4): L<<397.0,263.0>--<398.0,601.0>>
 * Adieresis (U+00C4): L<<398.0,0.0>--<397.0,263.0>> and 120 more. [code: found-semi-vertical]

</details>
<br>
</details>
<details>
<summary><b>[14] Foldit-ExtraBold.ttf</b></summary>
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
Glyph name: I	Contours detected: 2	Expected: 1
Glyph name: b	Contours detected: 1	Expected: 2
Glyph name: y	Contours detected: 2	Expected: 1
Glyph name: uni00B9	Contours detected: 2	Expected: 1
Glyph name: onehalf	Contours detected: 4	Expected: 3
Glyph name: Igrave	Contours detected: 3	Expected: 2
Glyph name: Iacute	Contours detected: 3	Expected: 2
Glyph name: Icircumflex	Contours detected: 3	Expected: 2
Glyph name: Idieresis	Contours detected: 4	Expected: 3
Glyph name: yacute	Contours detected: 3	Expected: 2
Glyph name: ydieresis	Contours detected: 4	Expected: 3
Glyph name: Itilde	Contours detected: 3	Expected: 2
Glyph name: Imacron	Contours detected: 3	Expected: 2
Glyph name: Ibreve	Contours detected: 3	Expected: 2
Glyph name: Idotaccent	Contours detected: 3	Expected: 2
Glyph name: ycircumflex	Contours detected: 3	Expected: 2
Glyph name: uni0208	Contours detected: 4	Expected: 3
Glyph name: uni020A	Contours detected: 3	Expected: 2
Glyph name: uni0233	Contours detected: 3	Expected: 2
Glyph name: uni1EC8	Contours detected: 3	Expected: 2
Glyph name: uni1ECA	Contours detected: 3	Expected: 2
Glyph name: ygrave	Contours detected: 3	Expected: 2
Glyph name: uni1EF5	Contours detected: 3	Expected: 2
Glyph name: uni1EF7	Contours detected: 3	Expected: 2
Glyph name: uni1EF9	Contours detected: 3	Expected: 2
Glyph name: uni20A6	Contours detected: 2	Expected: 1, 3 or 5
Glyph name: uni20A9	Contours detected: 5	Expected: 1, 3, 4 or 7
Glyph name: I	Contours detected: 2	Expected: 1
Glyph name: Iacute	Contours detected: 3	Expected: 2
Glyph name: Ibreve	Contours detected: 3	Expected: 2
Glyph name: Icircumflex	Contours detected: 3	Expected: 2
Glyph name: Idieresis	Contours detected: 4	Expected: 3
Glyph name: Idotaccent	Contours detected: 3	Expected: 2
Glyph name: Igrave	Contours detected: 3	Expected: 2
Glyph name: Imacron	Contours detected: 3	Expected: 2
Glyph name: Itilde	Contours detected: 3	Expected: 2
Glyph name: b	Contours detected: 1	Expected: 2
Glyph name: one	Contours detected: 2	Expected: 1
Glyph name: onehalf	Contours detected: 4	Expected: 3
Glyph name: uni0233	Contours detected: 3	Expected: 2
Glyph name: uni1EC8	Contours detected: 3	Expected: 2
Glyph name: uni1ECA	Contours detected: 3	Expected: 2
Glyph name: uni1EF5	Contours detected: 3	Expected: 2
Glyph name: uni1EF7	Contours detected: 3	Expected: 2
Glyph name: uni1EF9	Contours detected: 3	Expected: 2
Glyph name: uni20A6	Contours detected: 2	Expected: 1, 3 or 5
Glyph name: uni20A9	Contours detected: 5	Expected: 1, 3, 4 or 7
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
	* B (U+0042): L<<798.0,404.0>--<719.0,467.0>>/L<<719.0,467.0>--<952.0,274.0>> = 1.0645899864996058
	* asterisk (U+002A): L<<225.0,442.0>--<211.0,351.0>>/L<<211.0,351.0>--<271.0,730.0>> = 0.24975216281029114
	* d (U+0064): L<<822.0,309.0>--<821.0,310.0>>/L<<821.0,310.0>--<823.0,307.0>> = 11.309932474020227
	* dcaron (U+010F): L<<822.0,309.0>--<821.0,310.0>>/L<<821.0,310.0>--<823.0,307.0>> = 11.309932474020227
	* dcroat (U+0111): L<<822.0,309.0>--<821.0,310.0>>/L<<821.0,310.0>--<823.0,307.0>> = 11.309932474020227
	* dong (U+20AB): L<<812.0,313.0>--<809.0,316.0>>/L<<809.0,316.0>--<813.0,311.0>> = 6.3401917459097925
	* oe (U+0153): L<<1161.0,221.0>--<822.0,220.0>>/L<<822.0,220.0>--<822.0,220.0>> = 0.16901360862740877
	* p (U+0070): L<<36.0,221.0>--<39.0,218.0>>/L<<39.0,218.0>--<35.0,223.0>> = 6.340191745909908 and uni01C6 (U+01C6): L<<822.0,309.0>--<821.0,310.0>>/L<<821.0,310.0>--<823.0,307.0>> = 11.309932474020227 [code: found-jaggy-segments]

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
 * Euro (U+20AC): L<<324.0,333.0>--<824.0,334.0>>
 * Euro (U+20AC): L<<324.0,422.0>--<824.0,423.0>>
 * Euro (U+20AC): L<<847.0,310.0>--<324.0,309.0>>
 * Euro (U+20AC): L<<847.0,399.0>--<324.0,398.0>>
 * I (U+0049): L<<246.0,0.0>--<25.0,1.0>>
 * Iacute (U+00CD): L<<246.0,0.0>--<25.0,1.0>>
 * Ibreve (U+012C): L<<246.0,0.0>--<25.0,1.0>>
 * Icircumflex (U+00CE): L<<246.0,0.0>--<25.0,1.0>>
 * Idieresis (U+00CF): L<<246.0,0.0>--<25.0,1.0>>
 * Idotaccent (U+0130): L<<246.0,0.0>--<25.0,1.0>> and 75 more. [code: found-semi-vertical]

</details>
<br>
</details>
<details>
<summary><b>[14] Foldit-Light.ttf</b></summary>
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
Glyph name: A	Contours detected: 1	Expected: 2
Glyph name: I	Contours detected: 2	Expected: 1
Glyph name: b	Contours detected: 1	Expected: 2
Glyph name: q	Contours detected: 1	Expected: 2
Glyph name: y	Contours detected: 2	Expected: 1
Glyph name: section	Contours detected: 1	Expected: 2
Glyph name: uni00B9	Contours detected: 2	Expected: 1
Glyph name: onehalf	Contours detected: 4	Expected: 3
Glyph name: Agrave	Contours detected: 2	Expected: 3
Glyph name: Aacute	Contours detected: 2	Expected: 3
Glyph name: Acircumflex	Contours detected: 2	Expected: 3
Glyph name: Atilde	Contours detected: 2	Expected: 3
Glyph name: Adieresis	Contours detected: 3	Expected: 4
Glyph name: Igrave	Contours detected: 3	Expected: 2
Glyph name: Iacute	Contours detected: 3	Expected: 2
Glyph name: Icircumflex	Contours detected: 3	Expected: 2
Glyph name: Idieresis	Contours detected: 4	Expected: 3
Glyph name: yacute	Contours detected: 3	Expected: 2
Glyph name: ydieresis	Contours detected: 4	Expected: 3
Glyph name: Amacron	Contours detected: 2	Expected: 3
Glyph name: Abreve	Contours detected: 2	Expected: 3
Glyph name: Aogonek	Contours detected: 1	Expected: 2 or 3
Glyph name: Itilde	Contours detected: 3	Expected: 2
Glyph name: Imacron	Contours detected: 3	Expected: 2
Glyph name: Ibreve	Contours detected: 3	Expected: 2
Glyph name: Idotaccent	Contours detected: 3	Expected: 2
Glyph name: ycircumflex	Contours detected: 3	Expected: 2
Glyph name: uni0200	Contours detected: 3	Expected: 4
Glyph name: uni0202	Contours detected: 2	Expected: 3
Glyph name: uni0208	Contours detected: 4	Expected: 3
Glyph name: uni020A	Contours detected: 3	Expected: 2
Glyph name: uni0233	Contours detected: 3	Expected: 2
Glyph name: uni1EA0	Contours detected: 2	Expected: 3
Glyph name: uni1EA2	Contours detected: 2	Expected: 3
Glyph name: uni1EA4	Contours detected: 3	Expected: 4
Glyph name: uni1EA6	Contours detected: 3	Expected: 4
Glyph name: uni1EA8	Contours detected: 3	Expected: 4
Glyph name: uni1EAA	Contours detected: 3	Expected: 4
Glyph name: uni1EAC	Contours detected: 3	Expected: 4
Glyph name: uni1EAE	Contours detected: 3	Expected: 4
Glyph name: uni1EB0	Contours detected: 3	Expected: 4
Glyph name: uni1EB2	Contours detected: 3	Expected: 4
Glyph name: uni1EB4	Contours detected: 3	Expected: 4
Glyph name: uni1EB6	Contours detected: 3	Expected: 4
Glyph name: uni1EC8	Contours detected: 3	Expected: 2
Glyph name: uni1ECA	Contours detected: 3	Expected: 2
Glyph name: ygrave	Contours detected: 3	Expected: 2
Glyph name: uni1EF5	Contours detected: 3	Expected: 2
Glyph name: uni1EF7	Contours detected: 3	Expected: 2
Glyph name: uni1EF9	Contours detected: 3	Expected: 2
Glyph name: uni20A9	Contours detected: 6	Expected: 1, 3, 4 or 7
Glyph name: A	Contours detected: 1	Expected: 2
Glyph name: Aacute	Contours detected: 2	Expected: 3
Glyph name: Abreve	Contours detected: 2	Expected: 3
Glyph name: Acircumflex	Contours detected: 2	Expected: 3
Glyph name: Adieresis	Contours detected: 3	Expected: 4
Glyph name: Agrave	Contours detected: 2	Expected: 3
Glyph name: Amacron	Contours detected: 2	Expected: 3
Glyph name: Aogonek	Contours detected: 1	Expected: 2 or 3
Glyph name: Atilde	Contours detected: 2	Expected: 3
Glyph name: I	Contours detected: 2	Expected: 1
Glyph name: Iacute	Contours detected: 3	Expected: 2
Glyph name: Ibreve	Contours detected: 3	Expected: 2
Glyph name: Icircumflex	Contours detected: 3	Expected: 2
Glyph name: Idieresis	Contours detected: 4	Expected: 3
Glyph name: Idotaccent	Contours detected: 3	Expected: 2
Glyph name: Igrave	Contours detected: 3	Expected: 2
Glyph name: Imacron	Contours detected: 3	Expected: 2
Glyph name: Itilde	Contours detected: 3	Expected: 2
Glyph name: at	Contours detected: 1	Expected: 2
Glyph name: b	Contours detected: 1	Expected: 2
Glyph name: one	Contours detected: 2	Expected: 1
Glyph name: onehalf	Contours detected: 4	Expected: 3
Glyph name: q	Contours detected: 1	Expected: 2
Glyph name: section	Contours detected: 1	Expected: 2
Glyph name: uni0233	Contours detected: 3	Expected: 2
Glyph name: uni1EA0	Contours detected: 2	Expected: 3
Glyph name: uni1EA2	Contours detected: 2	Expected: 3
Glyph name: uni1EA4	Contours detected: 3	Expected: 4
Glyph name: uni1EA6	Contours detected: 3	Expected: 4
Glyph name: uni1EA8	Contours detected: 3	Expected: 4
Glyph name: uni1EAA	Contours detected: 3	Expected: 4
Glyph name: uni1EAC	Contours detected: 3	Expected: 4
Glyph name: uni1EAE	Contours detected: 3	Expected: 4
Glyph name: uni1EB0	Contours detected: 3	Expected: 4
Glyph name: uni1EB2	Contours detected: 3	Expected: 4
Glyph name: uni1EB4	Contours detected: 3	Expected: 4
Glyph name: uni1EB6	Contours detected: 3	Expected: 4
Glyph name: uni1EC8	Contours detected: 3	Expected: 2
Glyph name: uni1ECA	Contours detected: 3	Expected: 2
Glyph name: uni1EF5	Contours detected: 3	Expected: 2
Glyph name: uni1EF7	Contours detected: 3	Expected: 2
Glyph name: uni1EF9	Contours detected: 3	Expected: 2
Glyph name: uni20A9	Contours detected: 6	Expected: 1, 3, 4 or 7
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
	* section (U+00A7): L<<173.0,490.0>--<180.0,483.0>>/L<<180.0,483.0>--<73.0,636.0>> = 10.03312055433119 [code: found-jaggy-segments]

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
 * A (U+0041): L<<331.0,0.0>--<330.0,175.0>>
 * Aacute (U+00C1): L<<331.0,0.0>--<330.0,175.0>>
 * Abreve (U+0102): L<<331.0,0.0>--<330.0,175.0>>
 * Acircumflex (U+00C2): L<<331.0,0.0>--<330.0,175.0>>
 * Adieresis (U+00C4): L<<331.0,0.0>--<330.0,175.0>>
 * Agrave (U+00C0): L<<331.0,0.0>--<330.0,175.0>>
 * Amacron (U+0100): L<<331.0,0.0>--<330.0,175.0>>
 * Aogonek (U+0104): L<<331.0,0.0>--<330.0,175.0>>
 * Aring (U+00C5): L<<331.0,0.0>--<330.0,175.0>>
 * Aringacute (U+01FA): L<<331.0,0.0>--<330.0,175.0>> and 48 more. [code: found-semi-vertical]

</details>
<br>
</details>

### Summary

| 💔 ERROR | 🔥 FAIL | ⚠ WARN | 💤 SKIP | ℹ INFO | 🍞 PASS | 🔎 DEBUG |
|:-----:|:----:|:----:|:----:|:----:|:----:|:----:|
| 60 | 3 | 78 | 938 | 62 | 895 | 0 |
| 3% | 0% | 4% | 46% | 3% | 44% | 0% |

**Note:** The following loglevels were omitted in this report:
* **SKIP**
* **INFO**
* **PASS**
* **DEBUG**
