## Variables and Assignments expression ##
- **Variable** that store some value.
    -It will start with any letter
    -can contain any letter, number and puntuation except any white space.
    -name of variable can be anything, but being meaningful is prefered.
- **Assignments** operators is *=* sign.
    -  `variable_name = value`
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
    > :bulb: basically, any letter is of *char* (character) datatype. If we write a word or sentence, it will be of array of character type. *If we put this word or sentence inside a single quotation mark it will be recognized as array of character always. But, if we use double quotation mark it will be treated as **string** in MATLAB.*
---
- There are many type of data-type. 
    - numbers
        - integers:
            - *int8*, *int16*, *int32*, *int64*
                >This are for signed numbers meaning numbers with sign, either with positive or negative. 
            - *uint8*, *uint16*, *uint32*, *uint64*
                >This type does not store sign. That means all the numbers are thaught to be positive only
                >:bulb: as *signed integers* store both positive and negative values, it stores half of the positive numbers comparing *unsigned integers*. For example, if *unsigned integer* stores 0 to 255, then *signed integer* with same storage stores -128 to 127.   
        - fractional
            -there are two type of them: one is called *single* and another is *double*. *Double* is short for ***double precision***, meaning it stores for digits after decimal point.
            >Normally all the numbers, if not specified, it is stored as *double* type.
            a = 98
            class(a)
            #will return double.
            :question: how to specify data-type is discussed later.
    - characters
        - they are of either *char* or *string* type. But **Octave** only take *char* type data. It is not as updated as **Matlab**.
    - logical data-type
        - *true* and *false* values are of logical data-type.
---
&rightarrow;To specify any data-type we have to say it earlier before the data. <br>
    `variable_name = data_type (data)`
---
&rightarrow; The command used for watching the variables all declared is *who*. By using the command *whos*, the variables along with their data-type and their captured storage can be inspected.
 
        ```octave
        who         % will show all the variables.
        whos        % will show the full list with storage and data type.

&rightarrow; We can delete any variable by the command *clear*. If we use *clear* command, it will delete all the variables created. If we want to delete any specified variable it will delete this specified variable.
 
        ```octave
        variable_one = 1;
        variable_two = 2439;
        variable_three = 'c';
        variable_four = 'dance';

        clear variable_three        %only the third variable will be cleared.
        who                         %variable_one variable_two variable_four
        clear                       %will delete all the variables
        who                         %