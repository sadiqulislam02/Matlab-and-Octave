## Variables and Assignments expression ##

- **Variable** that store some value.
    -It will start with any letter
    -can contain any letter, number and puntuation except any white space.
    -name of variable can be anything, but being meaningful is prefered.
- **Assignments** operators is *=* sign.
  - `variable_name = value`
  - if value should be specified like int8, int16, uint32, it should be mentioned.
    - `variable_name = type (value)`
- **Variable Type** is accessed by the command *class* like `class (variable_name)` and it will return the type of the variable.
        ```octave
        a = 5
        class(a)
        # will return its type -> double
        # by-default any number is of 'double' type

        character = 'c'
        class(character)
        # char
        sentence = 'sadiqul'
        class(sentence)
        # char

        sen2 = "agarwal"
        class(sen2)
        #in octave -> char
        #in matlab -> string
    > basically, any letter is of *char* (character) datatype. If we write a word or sentence, it will be of array of character type. *If we put this word or sentence inside a single quotation mark it will be recognized as array of character always. But, if we use double quotation mark it will be treated as **string** in MATLAB.*
  >
---
&rightarrow; There are
