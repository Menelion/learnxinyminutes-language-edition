# Contributing

All contributions are welcome, from the tiniest typo to a brand new article. Translations in all languages are welcome (or, for that matter, original articles in any language). Send a pull request or open an issue any time of day or night. Pull Requests will remain open for a minimum of approximately 24 to 48 hours to allow for discussion and review. This is subject to change.

**Please prepend the language codes to your issues and pull requests**.

Examples:

- [en-eo] The English to Esperanto Issue
- [en-eo] The English to Esperanto Pull Request

We're happy for any contribution in any form, but if you're making more than one major change (i.e. translations for two different languages) it would be super cool of you to make a separate pull request for each one so that someone can review them more effectively and/or individually.

## First Steps

- [ ] Fork this repo
- [ ] Create your feature branch (usually based on the languages you are working on)
- [ ] Add your feature (See below)
- [ ] Submit a pull request

## How to Add a New Language

- [ ] Add a new Markdown file under `_languages` using the `templates/new-language.md` file as a template
    - Replace the following:
        - `{---}` with `---`
        - `{YOUR_NAME}` with the name you want displayed. Please refer to the [Code of Conduct](../CODE_OF_CONDUCT.MD)
        - `{LANG_CODE_1}` with the ISO 639-1 code for the original language
        - `{LANG_CODE_2}` with the ISO 639-1 code for the translated language
        - `{LANG_NAME_1}` with the ISO 639-1 name for the original language
        - `{LANG_NAME_2}` with the ISO 639-1 name for the translated language
    - Example file name: `en-es.md`
- [ ] Create a new directory under `_data` with the language codes.
    - Example: `en-es`
- [ ] See below for [How to Add to a Language](#how-to-add-to-a-language)

## How to Add to a Language

- [ ] Create a new section file under the correct `_data` directory using the language codes as defined in ISO 639-1
    - Example: `basics.json`(preferred) or `basics.csv` or `basics.yml` or `basics.yaml`
    - For more information:
      - [JSON Example](https://en.wikipedia.org/wiki/JSON#Example)
      - [CSV Example](https://en.wikipedia.org/wiki/Comma-separated_values#Example)
      - [YAML Example](https://en.wikipedia.org/wiki/YAML#Example)

## Style Guide

- **Add a newline at the end of the file**
- **Keep examples simple**: Use a few words or a short sentence that will translate fairly simple across multiple languages
- **Basic concepts welcome**: This is aimed at language beginners (for now)
- **Use UTF-8**: Try to leave out the byte-order-mark at the start of the file. (:set nobomb in Vim) - You can check if the file contains a BOM on Linux/Unix systems by running `file YOUR-FILE-NAME.EXT`. You will see this if it uses a BOM: UTF-8 Unicode (with BOM) text

## Should I add myself as a Contributor?

If you want to add yourself to contributors, keep in mind that contributors get equal billing, and the first contributor usually wrote the whole file. Please use your judgement when deciding if your contribution constitutes a substantial addition or not. If you believe this to be the case then add your info to the README under Contributors in the correct list!

**Note**: *Add your name to the bottom of the correct list only once and don't reorder it unless you are a maintainer. Thanks!*
