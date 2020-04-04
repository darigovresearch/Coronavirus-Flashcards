# Contributing
To make this project extensible as far into the future as possible we are following certain rules which will also make it possible to programmatically pull the data.

Pull requests, corrections & fixes are welcome. Any contributions must be submitted under the same license that the original piece of work (see below). Take a look at any open issues or submit new ones if there is something that needs to be fixed or added.

## Folder and Filename conventions
Every language should be saved in a folder called `lang-code` for example `[fr]` for French. In each folder you save
- .csv source files for each chapter
- and a folder called `APKG`

The latter is for the output .apkg files after having imported and exported the .csv files via Anki.

**Each chapter name .csv file has five parts to it:**
1. Coronavirus Flashcards
2. fr
3. Français
4. Chapter X
5. Chapter title
6. .csv

**Explanation**
1. is literally `Coronavirus Flashcards` translated into the language that the flashcards are in,
2. is the language code for the given language,
3. the full language name translated in the given language
4. is "Chapter X" is "Chapter" translated into the language followed by the chapter number (1, 2, 3 etc),
5. is the chapter title translated into the language,
6. is the extension file to make it readable by the correct text editors & other computer programs (here it is a csv file)

**Each chapter name .apkg file has eight parts to it:**
1. Coronavirus Flashcards
2. fr
3. Français
4. (Darigov Decks)
5. Chapter X
6. Chapter title
7. .apkg

**Explanation**
1. is literally `Coronavirus Flashcards` translated into the language that the flashcards are in,
2. is the language code for the given language,
3. the full language name translated in the given language
4. a way to designate that the Anki Flashcards comes from a larger body of work (Darigov Decks, see our other works),
5. is "Chapter X" where the word "Chapter" is translated into the language followed by the Chapter number (1, 2, 3 etc),
6. is the Chapter title translated into the language,
7. is the extension file to make it readable by Anki-based software (here it is an Anki Package file)


### Translating for other languages
Translations in all languages are welcome. Send a pull request or open an issue any time of day or night.

**Please prepend the tag `[lang-code]` to your issues and pull requests.** For example, `[fr]` for French. This will help everyone pick out things they care about.

We're happy for any contribution in any form, but if you're making more than one major change (i.e. translations for two different languages) it would be super cool of you to make a separate pull request for each one so that someone can review them more effectively and/or individually.

## Requesting a new language
You can request a language via an issue request with the following title `[lang-code]: Language Request` and body text:

```
*New language* has been requested, having the following title names in *New language* to build out the folder structure would be helpful to begin the translation of each chapter

1. Glossary of terms
2. History of Epidemics
3. Biology
4. Medicine
5. Mathematics
6. Manufacturing & Logistics
7. Public Policy
8. Sociology
9. Academia
10. Appendix - Flashcards FAQs
11. Appendix - Coronavirus FAQs
12. Appendix - Corrections

Other terms
1. Coronavirus Flashcards
2. Introduction
```

Supplying the new language translation of all the chapter titles means that we can create the corresponding folder structure & to make it easier for you to just translate the content. In the future we hope to have code to auto generate the file structure for you but this is currently work in progress.

## File structure
Each file has one row for each word or phrase separated by a `|` where the text on each side corresponds to the front & back of the flashcard.

The first card of the main deck contains an introductory card. It is very important as if it is not visible the user will not know where they can find updates, corrections and improvements to the flashcards.

Please work from the first to the last section for consistency when translating into a new language as it also means that some can learn using your translation before having all the sections. However translating the Glossary of terms, Flashcard FAQs & Coronavirus FAQs would probably provide the most help from the start.

## Steps for submitting a new translation
The general process for porting existing translations to make a new language is the following:
1. Make a fork of the latest version of the repository
2. Download it to your local computer
3. Copy the source files which contains definitions in a language that you speak
4. Rename the filename translating the correct words if required
5. Translate the front of each card along with it's explanation
6. Check your work (it is much easier to make corrections before many people have downloaded your translated flashcards than after)
7. Generate the .apkg file with the correct filename in the app
    - Do so in a fresh desktop Anki profile to ensure that as many new words are imported as possible
8. Make a pull request

## Style Guidelines
- Do make sure punctuation is consistent across translations
    - This includes but is not limited to spaces, brackets, quotation marks, question marks, asterisks, exclamation points, ellipses etc.
- Do follow the naming conventions for file and folder names above
- Do ensure that you are using the correct delimiter on each row
- Do not delete or combine multiple translations into one line
- Refrain from adding additional context to a translation as it may not be relevant
- Do not use any online translation tools or dictionaries to help with the translation
    - We want this project to be a human-led endeavour as people tend to understand the context of translation better than computer generated tools
