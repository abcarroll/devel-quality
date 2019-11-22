# Develop QA-Quality

This is a temporary placeholder.  Much more to come.

Currently, the following in the works:

 - Standardizing conf files across most tools (phpstan, psalm, etc)
 - Easily keep routines/scripts/tasks/code standard configurations for projects and your own personal setups versioned
 and standardized, auto-loaded.
 - Make it easy to actually use QA/Testing tools.

## Roadmap 

I really don't have much time to devote to this project, however:

 - [ ] Create a system whereby similar rules between different tools can be grouped into both fine and high-level "profiles"
 of sorts.  Most tools go from "how exactly do you want the opening bracket of an array access after the 16th character
 on a tuesday to be placed?" to "PSR-2...ish" and nothing inbetween.  Additionally, these should be grouped into "whitespace",
 "formatting", "very safe" (bad things into good things with no functional changes, e.g. backtick usage), "safe" (virtually no
 risk involved except perhaps archaic php versions or extreme edge cases), "moderately safe" (rarely should cause issue), unsafe
 (could on occasion cause issues), and very unsafe (very frequently would cause issues unless very carefully configured; e.g. 
 removal of unused publics).
 - [ ] Create a script to dynamically dump out all rules for tools:
   - [ ] phpcs
   - [ ] php-cs-fixer
   - [ ] psalm/psalter
   - [ ] phpmd (?)
 - [ ] Tool to run each tool intelligently as to be able to review a diff beforehand
   - [ ] File by file
   - [ ] Rule by rule 
 - [ ] This tool can generate configs
 - [ ] See ab/develop-stack (similar needed): Tool to launch httpd on local system; then launch browser, don't launch multiple 
 instances of browser.
 
MIT Licensed.
