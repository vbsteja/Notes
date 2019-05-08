### Regex Notes

* grep -i "license" GPL-3  --> search for text containing word with case insensitive.

* grep -v "the" BSD  --> search for the text not containing word

* grep "^GNU" GPL-3  --> Anchor Match, match the start of the line with word

* grep "and$" GPL-3  --> End Match, match the end of the line with word

* grep '..cept' GPL-3  --> matching any character with a dot(.)

* grep 't[wo]o' GPL-3 --> matching any of the character inside the bracets with a word in the text.

* grep '[^c]ode' GPL3  --> except the character inside the bracket.

* grep "^[A-Z]" GPL-3 / grep "^[[:upper:]]" GPL-3  --> match a line that start with a capital letter.

* grep "([A-Za-z ]*)" GPL-3 -->  matching characters repeating zero or more times.


* grep "^[A-Z].*\.$" GPL-3  --> escape character usage.

## Examples from regex101:

* to find the text contains both letters and digits,special characters, useful for cipher text detection.
     * ** (?=\d*[a-zA-Z])(?=[a-zA-Z]*[\d+])[a-zA-Z\d]+ **
