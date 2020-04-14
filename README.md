Style linter for Rapid7 UX Writing Team. 

## Vale commands when running locally.

* Test all markdown files (.md) in the current directory (.):
 `vale --glob='*.md' .`
* To test a single file `vale filePath/fileName`

## Vale documentation 
https://errata-ai.gitbook.io/vale/

## Setup

* Configuration file must be named `.vale.ini` or `_vale.ini` and needs to be at th*e top level directory. 
* Styles files are written in `yml` and located in `.github/valeStyles`.
* `test_docs` - test all the rules configured.

## To do

- [ ] Add links to the rule it references in each yaml file. Left off since final location is not decided on.
- [ ] Trying to figure out of I can check for sequential headings. I have not figured it out yet.[.github/valeStyles/SequentialHeadings.yml](.github/valeStyles/SequentialHeadings.yml)
- [ ] Figure out checking for empty headings (.github/valeStyles/EmptyHeadings.yml)[.github/valeStyles/EmptyHeadings.yml] Current regex only checks for the heading, it doesn't check to see if its empty and it only checks the first line. 
- [ ] Fill in positive and negative language. [.github/valeStyles/PostiveLanguage.yml](.github/valeStyles/PostiveLanguage.yml)

## Styles I skipped
The following is a list of guidelines I skipped because I couldn't figure out how to check for them

* Identity first language- I think I can check for this, but need a table of terms to look for. 
* Need more slang. Only have a few, but its meant to capture all slang/ [.github/valeStyles/Slang.yml](.github/valeStyles/Slang.yml)

## Regex
Need to build a regex expression to match on: http://buildregex.com/
Need to test it out: https://regexr.com/

