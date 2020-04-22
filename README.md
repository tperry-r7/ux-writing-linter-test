# Style linter for Rapid7 UX Writing Team. 
Contains the vale configuration files for R7 style guide linter. 

## Vale commands when running locally.
* Test all markdown files (.md) in the current directory (.): `vale --glob='*.md' .`
* To test a single file:  `vale filePath/fileName`

## Vale documentation 
https://errata-ai.gitbook.io/vale/

## Setup

* Configuration file must be named `.vale.ini` or `_vale.ini` and needs to be at the top level directory. 
* Styles files are written in `yml` and located in `.github/valeStyles`.


## To do

- [ ] Change links to final style guide
- [ ] Trying to figure out of I can check for sequential headings. [test_docs/rules_in_progress/SequentialHeadings.yml](test_docs/rules_in_progress/SequentialHeadings.yml)
- [ ] Figure out checking for empty headings (test_docs/rules_in_progress/EmptyHeadings.yml)[test_docs/rules_in_progress/EmptyHeadings.yml]
- [ ] Check for empty links  [test_docs/rules_in_progress/EmptyLinks.yml]()
- [ ] Check for italics [test_docs/rules_in_progress/Italics.yml](test_docs/rules_in_progress/Italics.yml)
- [ ] Can I check for a lead in sentance to lists? I think that might be a script and not vale
- [ ] External Links on a new line [test_docs/rules_in_progress/NewLineLinks.yml]()
- [ ] Fill in positive and negative language. [.github/valeStyles/PostiveLanguage.yml](.github/valeStyles/PostiveLanguage.yml)
- [ ] Underlined words and phrases can look like links, so don’t underline for emphasis.
- [ ] Figure out how to test for the second abbreviation. .github/valeStyles/MeasurementAbbreviations.yml
- [ ] Need more slang. Only have a few, but its meant to capture all slang/ [.github/valeStyles/Slang.yml](.github/valeStyles/Slang.yml)


## Regex
Need to build a regex expression to match on: http://buildregex.com/
Need to test it out: https://regexr.com/, https://regex101.com/

# FAQ
1. I keep getting output, but the article is fine. What do I do?
  - Nothing. This is meant to be a suggestion and bring your attention to something. If a rule exists you should review it 
  and see if it applies to you. If it is non negotiable then its returned as an error. 
2. I want to make a new rule or changes.
  - Review the Vale docs. Mostly https://errata-ai.gitbook.io/vale/getting-started/styles#introduction and https://errata-ai.gitbook.io/vale/getting-started/markup#available-scopes. Also look at the third party resources for inspiration. https://github.com/errata-ai/styles