Styles Linter for Rapid7 UX Writing Team. 

## Vale commands when running locally.

* Test all markdown files (.md) in the current directory (.):
 `vale --glob='*.md' .`
* To test a single file `vale filePath/fileName`

## Vale Documentation 
https://errata-ai.gitbook.io/vale/

## Setup

* Configuration file must be named `.vale.ini` or `_vale.ini` and needs to be at th*e top level directory. 
* Styles files are written in `yml` and located in `.github/valeStyles`.
* `test_docs` - test all the rules configured.

## To Do

- [ ] Add links to the rule it references in each yaml file. Left off since final location is not decided on.
