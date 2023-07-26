# UTF-8 Validation
A character in UTF8 can be from 1 to 4 bytes long, subjected to the following rules: For a 1-byte character, the first bit is a 0 , followed by its Unicode code. For an n-bytes character, the first n bits are all one's, the n + 1 bit is 0 , followed by n - 1 bytes with the most significant 2 bits being 10 .
![image](https://github.com/ugoem/alx-interview/assets/24642339/62feb288-abf7-4ebd-bcf7-e41fdbc4649f)


# Resources
* Read or watch:
* UTF-8 Characters, Symbols, and the Unicode Miracle

# Requirements
## General
* Allowed editors: vi, vim, emacs
* All your files will be interpreted/compiled on Ubuntu 14.04 LTS using python3 (version 3.4.3)
* All your files should end with a new line
* The first line of all your files should be exactly #!/usr/bin/python3
* A README.md file, at the root of the folder of the project, is mandatory
* Your code should use the PEP 8 style (version 1.7.x)
* All your files must be executable
