# Community translations for Caveblazers!
### How to contribute
- Create your own **fork** of the main repository
- Download the files & make changes where you see fit
- Commit your changes to your fork
- When you're ready to merge your changes, create a **pull request** from your fork in to the main repository

There's a [Google Sheet](https://docs.google.com/spreadsheets/d/1gwRiBYikRrkdn3Jlg9Q-LY_lg19Mxzfg4KG4jiX7eBg) available with all of the game's text: https://docs.google.com/spreadsheets/d/1gwRiBYikRrkdn3Jlg9Q-LY_lg19Mxzfg4KG4jiX7eBg

You can't edit the Google Sheet, but you can use it as a reference when translating the json files.

#### Guidelines
- Make sure you save your language files with **UTF-8 encoding** after making any changes! Otherwise most accents & special characters won't work.

- Anything within `{curly brackets}` should not be translated. For example `+10 {Melee Damage}` should be kept in English. However the ordering can be altered if `{Melee Damage} +10` makes more sense in the given language.

- Magic item descriptions contain a `-USE-` tag. This should not be translated. It is used in game to split items' descriptions and "use descriptions".
For example:
```
A gold skull which follows you around.-USE-the golden skull attacks nearby targets.
```
will be shown in game as:
```
A gold skull which follows you around.

Use:
The golden skull attacks nearby targets.
```
- Newlines can be added to text by entering `\n`. The game will generally add newlines automatically, but this can be useful for item/blessing/perk descriptions.
- All dialogue lines can be made plural by adding an "s" to the end of the tag. e.g:
```
"tutorial1_3": "Get up here, fella",
"tutorial1_3s": "Get up here, fellas",
```

### How to install a language file
1. Get Caveblazers on [Steam](http://store.steampowered.com/app/452060/Caveblazers/), [Humble](https://www.humblebundle.com/store/caveblazers) or [GOG](https://www.gog.com/game/caveblazers)
2. Download the language file that you want to use (e.g. Russian_RU.json)
3. Go to your Caveblazers folder (e.g. Steam\steamapps\common\Caveblazers) and put the language file in to the "Languages" folder
Open up the **languages.ini** file in your favourite text editor and add the language name, and file path to the list. e.g:
```
[1]
name = "English"
file = "Languages/English_GB.json"
[2]
name = "Russian"
file = "Languages/Russian_RU.json"
```
4. Caveblazers currently supports Chinese, Japanese and Russian characters (more to come), but in order for the game to use the correct font, your language filename must end in **_RU** for Russian, **_JA** for Japanese, and **_ZH** for Chinese.
5. Open up the game, and go to the Game Settings, if you have more than one language file in your Language folder and in your languages.ini file then you should have an option to change your language

### Known Issues
- A lot of non-english text does not fit in to certain windows (e.g. inventory, perk selection, journal, etc)
- Cutscenes have linebreaks & pauses that make sense in English, but may not make sense in other languages

If you find any other issues (unsupported characters, for example), you can report them on the [GitHub Issues](https://github.com/wlewisgames/caveblazers-translations/issues) section.
