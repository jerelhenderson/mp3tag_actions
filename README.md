# MP3TAG Tag Actions

## About MP3TAG
[MP3TAG](https://www.mp3tag.de/en/) is a powerful, freeware audio metadata editor,
supporting a number of different file formats. The versatility of the software is 
made available through use of [Actions](https://help.mp3tag.de/options_format.html), which
take advantange of MP3TAG's built-in tools to perform edits on file tags, filenames... or
even folder paths. For example, one could use *Case Conversion* to convert all the ALBUM tags
from a file list to uppercase.

<p align="center">
<img src="/images/case_conversion.png" alt="Case Conversion Example"/>
</p>

While MP3TAG comes equipped with a number of self-explanatory *Actions*, combining *Actions* with
[regular expressions](https://regexone.com/) and MP3TAG's built-in [scripting functions](https://help.mp3tag.de/main_scripting.html) is the key to unlocking the door of the power behind the program. Furthermore, *Actions* can be 
combined into sets called *Action Groups*, where multiple distinct actions are performed at once. 
*Action Groups* make editing hundreds or more files a cinch.

This repository is a collection of MP3TAG *Actions* I use to clean newly acquired music files
to prepare for introduction into my music library. 

## Installation
1. [Download MP3TAG](https://www.mp3tag.de/en/download.html) *v2.94 or later required*
2. Download the [repository](https://github.com/jerelhenderson/mp3tag_actions/archive/refs/heads/main.zip)
3. Unpack the archive into the `...\Data\Actions` folder
* Windows 10 `C:\Users\ %username% \AppData\Roaming\Mp3tag\Data\Actions`
* Windows XP `C:\Documents and Settings\ %username% \Application Data\Mp3tag\Data\Actions`
* Portable Install `%mp3tag%\Data\Actions`

## Additional
***Actions* follow numerical ordering when executing on files.**
Some *Actions* are numbered in accordance to the tags they affect. Changing either of these number orders
will result in tagging errors. I have included the *Action Group* preset `Normal Complete.mtg` which ticks
ll *Actions* used to clean and order tags in my collection.

My music manager of choice is [MusicBee](https://getmusicbee.com/)
and some *Actions* address it specifically. Users of other managers will likely need to make changes
consistent with their music manager or playback software. As well, an even smaller number of *Actions* assume
tag formatting consistent with [MusicBrainz Style Guidelines](https://musicbrainz.org/doc/Style), but some handling
is done to safely refrain from changes if the formatting is unexpected.

