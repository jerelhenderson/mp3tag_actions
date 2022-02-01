## Tag Actions

### Grammartron
[Grammartron](https://community.mp3tag.de/t/case-conversion/11684) is a comprehensive, collective effort among the
MP3TAG community to format, fix and standardize spellings and grammatical issues in music tags.
<ul style="list-style: none;">
<li>01 Grammartron - Smart Case and Grammar Restorer #1 - Tags.mta</li>
<li>01 Grammartron - Smart Case and Grammar Restorer #2 - Filenames.mta</li>
<li>01 Grammartron - Smart Case and Grammar Restorer #3 - Parent Directory.mta</li>
</ul>

### Track counters
Supplements built-in track counter
<ul style="list-style: none;">
<li>02 Track Counter #1 - Track Number.mta</li>
	- prepend incrementing track numbers to total file number
<li>02 Track Counter #2 - Track Total.mta</li>
	- append total file count to track numbers
<li>02 Track Counter #3 - Both.mta</li>
	- increment track numbers and appending total file count
<li>02 Track Counter #4 - Vinyl (Letters).mta</li>
	- increment vinyl-style track numbers (A01... B01...), set DISCSUBTITLE to "Side A... Side B..."
<li>02 Track Counter #5 - Vinyl (Numbers).mta</li>
	- set DISCSUBTITLE to "Side 1... Side 2..."
</ul>

### Parse featured artists
Split featured artists in ARTIST or TITLE to GUEST ARTIST
<ul style="list-style: none;">
<li>03 Guess featured artists from title, artist.mta</li>
</ul>

###  Perform various edits to ARTIST, ALBUMARTIST and PERFORMER tags
<ul style="list-style: none;">
<li>04_1 Convert GUEST ARTIST to PERFORMER.mta</li>
	- copy tags in GUEST ARTIST to PERFORMER
<li>04_2 Switch ALBUMARTIST and ARTIST.mta</li>
	- swap ALBUMARTIST and ARTIST tags
<li>05_1 ARTIST or PERFORMER to ALBUMARTIST.mta</li>
	- copy ARTIST to ALBUMARTIST, unless specific requirements (for classical tracks) are met
<li>05_2 ALBUMARTIST (and-or COMPOSER) to ARTISTSORT.mta</li>
	- copy ALBUMARTIST to ARTISTSORT, and attach COMPOSER if STYLE=Classical
</ul>

### Miscellaneous naming corrections
Additional naming and grammatical style corrections not included in Grammartron
<ul style="list-style: none;"> 
<li>06 More Naming and Style Corrections.mta</li>
</ul>

### Format ARTIST/COMPOSER and the like
<ul style="list-style: none;">
<li>07_1 Copy ARTIST to COMPOSER, create DISPLAY COMPOSER.mta</li>
	- if ARTIST meets certain conditions, copy to COMPOSER, DISPLAY COMPOSER from COMPOSER, format (mostly if STYLE=Classical)
<li>07_2 Create DISPLAY COMPOSER.mta</li>
	- create DISPLAY COMPOSER
<li>08_1 Convert separators to ; and SPLIT #1 - ARTIST.mta</li>
	- delimiters in ARTIST are converted to semi-colons, then split into a multi-tag
<li>08_2 Convert separators to ; and SPLIT #2 - COMPOSER LYRICIST.mta</li>
	- delimiters in COMPOSER and LYRICIST are converted to semi-colons, then split to a multi-tag
<li>09 Create DISPLAY ARTIST, format DISPLAY ARTIST.mta</li>
	- create DISPLAY ARTIST from ARTIST, format 
</ul>

### Zero Width Whitespace LANGUAGE
Remove LANGUAGE, unless STYLE is "Classical" and remove superfluous COMMENT tags
<ul style="list-style: none;">
<li>11 Remove LANGUAGE-COMMENT.mta</li>
</ul>

### Duets
Replace 'and' with ampersand in DISPLAY ARTIST
<ul style="list-style: none;">
<li>12 Do-ets.mta</li>
</ul>

### ALBUM Parentheses to Colon
Per the MusicBrainz Style Guide, convert albums with subtitles inside parentheses to colons
For example, "Planet of the Apes (Original Sound Track)" becomes "Planet of the Apes: Original Sound Track"
<ul style="list-style: none;">
<li>13 ALBUM (Subtitle) to Colon.mta</li>
</ul>

### Make iTunes compilation
Copy ALBUMARTIST to ARTISTSORT, then set COMPILATION=1
<ul style="list-style: none;">
<li>14 ALBUMARTIST to ARTISTSORT, then blank ALBUMARTIST  (for compilations).mta</li>
</ul>

### Soundtrack creation tags
Create tags that designate an album as a soundtrack album, with the ability to sort albums part of a television or movie series
<ul style="list-style: none;">
<li>15 Add MOVIEORALBUM and ARTISTSORT.mta</li>
<li>15 Soundtrack Album Modifier.mta</li>
<li>15 Soundtrack Sorter.mta</li>
  - Add ZWSP characters in front of ALBUMSORT to custom sort albums. For example, the Star Wars Prequel Trilogy comes after the Original Trilogy in real world chronology, but in-universe they occur before.
</ul>

### Tags for cataloging pre-modern popular music
If STYLE=Classical, applicable and useful information is extracted from a text file and from the TITLE into separate tags
<ul style="list-style: none;"> 
<li>17 Period and Subperiod.mta</li>
  - Pulls a list of composers and their lifespans from a text file, isolates the relevant composer for the track and sets a corresponding PERIOD and SUBPERIOD
<li>18 Find the INITIALKEY and PROPERKEY.mta</li>
<li>18 Find the TEMPI.mta</li>
<li>19 Find the MOVEMENT.mta</li>
<li>19 MOVEMENTTOTAL.mta</li>
</ul>

### Arabic<->Roman Numerals Conversion
Convert Arabic numerals to Roman numerals and vice versa
<ul style="list-style: none;">
<li>20 Arabic Number to Roman Rumeral.mta</li>
<li>20 Convert NUM_ARAB to MOVEMENT.mta</li>
<li>20 Convert NUM_ARAB to MOVEMENTTOTAL.mta</li>
<li>20 Roman Numeral to Arabic Number.mta</li>
</ul>

### Create and format various year and date tags
Format YEAR tag based on file type, as well as setting the ORIGINAL YEAR and ORIGINALDATE tags based on album type
<ul style="list-style: none;">
<li>21 Split YEAR.mta</li>
</ul>

### PERFORMER & INVOLVEDPEOPLE tag formatting
<ul style="list-style: none;">
<li>22 PERFORMER edits #1 - Normal.mta</li>
<li>22 PERFORMER edits #2 - Wikipedia.mta</li>
<li>22 PERFORMER edits #3 - Discogs.mta</li>
<li>22_4 Convert PERFORMER to GUEST ARTIST.mta</li>
<li>22_5 Split INVOLVEDPEOPLE to GUEST ARTIST.mta</li>
<li>22_6 Split INVOLVEDPEOPLE to distinct tags.mta</li>
<li>22_7 Split INVOLVEDPEOPLE to PERFORMER(s).mta</li>
<li>22_8 Split INVOLVEDPEOPLE to ARTIST.mta</li>
<li>22_9 Reattach CONTRIBUTORS.mta</li>
</ul>

### Disc Folder Creator
Move tracks to separate disc folders if they're not already separated
<ul style="list-style: none;">
<li>23 Disc Maker.mta</li>
</ul>

### Clean Up Tags
Miscellaneous cleanup of unneeded and unnecessary tags, remove duplicated information in multi-tags and check for RELEASECOUNTRY · PUBLISHER CATALOGNUMBER · MEDIA TYPE/SOURCE MEDIUM before formatting
<ul style="list-style: none;">
<li>24_1 Picard Fixes.mta</li>
<li>24_2 Fix Duplicates, Split Combined Tags.mta</li>
<li>24_3 Album Details Creator.mta</li>
</ul>

### Add "Soundtrack" to STYLE if missing
Append "Soundtrack" to STYLE, if missing and album is a soundtrack
<ul style="list-style: none;">
<li>25 Attach 'Soundtrack' to STYLE.mta</li>
</ul>

### Format track filenames
<ul style="list-style: none;">
<li>26 Validate Filenames.mta</li>
</ul>

### Format and move albums
<ul style="list-style: none;">
<li>27 Normal Folder Renamer.mta</li>
<li>27 Singles Folder Renamer.mta</li>
<li>27 Soundtrack Folder Renamer.mta</li>
</ul>

### Format and move classical tracks
Move `STYLE==Classical` tracks from staging folder to music library</br>

Directory path roughly follows the format below...</br>
`Drive Letter :\ Classical \  PERIOD \ SUBPERIOD \ <Sort Composer> (LIFESPAN) \ <Genre> \ <Album Artist> - $If(<Original Year>=<Year (yyyy)>,(<Year (yyyy)>),(<Original Year>) (<Year (yyyy)>)) - <Album> $If($IsMatch(<ENSEMBLE>,"(orchestra|choir):"),(<ENSEMBLE>),) [RELEASECOUNTRY · PUBLISHER CATALOGNUMBER · SOURCE MEDIUM]`<br/>
Presenting results such as...<br/>
`M:\Classical\Classical era\Middle\Bologne, Joseph (1745-1799)\Concerto\Rachel Barton Pine (violin) - (1997) Violin Concertos by Black Composers of the 18th and 19th Centuries (Encore Chamber Orchestra) [US · Cedille CDR 90000 035 · CD]`<br/>
<ul style="list-style: none;">
<li>28 Move Classical Albums.mta</li>
</ul>

### Remove multiple embedded album covers
Strip multiple embedded album covers from tracks, then re-embeds just the front cover
<ul style="list-style: none;">
<li>29 Album Cover Fix.mta</li>
</ul>

### Preset
*Action Group* presets allow switching of various *Action* sets. Newly added albums are processed first 
with this preset and most can be moved to the main library immediately following.
<ul style="list-style: none;">
<li>Normal Complete.mtg</li>
</ul>
