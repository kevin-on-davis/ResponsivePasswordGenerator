# ResponsivePasswordGenerator
# Homework #3

## Overview
The assignment issued was to create a random password generator which accepts as user input
* Length (must be between 8 and 128 characters)

* Character type:

  * Special characters ([see examples](https://www.owasp.org/index.php/Password_special_characters))

  * Numeric characters

  * Lowercase characters

  * Uppercase characters

The application should validate user input and ensure that at least one character type is selected.


## Key skills for reinforcement
* Javascript programming
* Document Object Model (DOM)
* Event Listeners
* Arrays
* Math object (specifically Math.random)

## Implementation
The password is being generated by two methods each based on reading the ASCII table to generate the required password one character at a time.
* direct conversion - random integers between 33 and 126 were generated using Math.random and the corresponding ASCII characters were constructed into the  password string. Characters matching the character types not selected by the user are excluded from the string as it is being constructed.
* array processing - an array is populated by ASCII characters based on the character types selected by the user. Random integers between 0 and the length of the array (less 1) are generated to represent array index values which are used to select array content values identified by the index value.
