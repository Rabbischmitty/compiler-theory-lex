# Compiler Theory Lexical Analyzer
Contains a school project to create a lexical analyzer using flex, bison, C++, and make. The aim of the course was to explore what actions the compiler takes during its various phases.

We were given a skeleton file that demonstrated basic syntax in Bison and C++, and asked to add additional basic features to include recognition of hex and real values.

## Requirements
- Your favorite Linux distribution (I recommend Ubuntu for this project)
- Use `apt` or `yum` to get the packages for Flex, Bison, Make, and G++ (Use `sudo` to avoid permission issues)
- Create your desired directory for the files using `mkdir`
- Move source files to your chosen directory using `mv` or your personally prefered method
- Navigate to the directory with the source files and use `make` to compile the project
- Utilize the following syntax to run the program `./compile < test1.txt`

## Features Added
- Added reserved words for `else, elsif, endfold, endif, fold, if, left, real, right, then`
- Added all functionality for logical operators for `!` and `|`
- Added all functionality for relational operators `=`, `<>`, `>`, `>=`, and `<=`
- Added lexemes for `-` and `/`
- Added all functionality for modulus operator `%`
- Added all functionality for exponent operator `^`
- Added all functionality for unary minus operator `~`
- Added recognition of additional comments using `--`
- Allowed for underscores to be recognized
- Restricted underscores to no more than two consecutive underscores with no leading or trailing underscores
- Added all functionality for hexadecimal values
- Added all functionality for real values
- Added recognition for escape characters `\b`, `\t`, `\n`, `\r` and`\f`

### Special Notes
- If you are modifying any of the files, you must run `make` to compile your new changes
- If you are modifying the `scanner.l` you must modify the `tokens.h` to recognize the new token.
- Included test cases can be accessed via the **tests** folder in the repo
