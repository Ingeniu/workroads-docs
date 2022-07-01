# Functions

## Mathematics

### Round

#### Description

The Round function rounds a number to a specific number of digits or to a specific fraction or multiple

#### Syntax

```
=Round(number, [rounding_step], [rounding_offset])
```

| Arguments       | Req/Opt  | Description                                                  |
| --------------- | -------- | ------------------------------------------------------------ |
| number          | Required | Number to round                                              |
| rounding_step   | Optional | Digit, fraction or multiple to which you want to round the number. |
| rounding_offset | Optional | Allows to add an offset in the rounding of a number.         |

#### Examples

| Formula            | Result | Description                                                  |
| ------------------ | ------ | ------------------------------------------------------------ |
| =Round(3.49)       | 3      | Rounds to the nearest integer                                |
| =Round(3.5)        | 4      | Rounds to the nearest integer                                |
| =Round(123.45,0.1) | 123.5  | Rounds to one decimal place                                  |
| =Round(123.45,10)  | 120    | Rounds to the nearest 10                                     |
| =Round(53,12)      | 48     | Rounds to the nearest dozen. Useful to pack eggs, beers and other things of the kind. |
| =Round(53,13)      | 52     | Rounds to the nearest multiple of 13. Allows you to pack your eggs in a package of 13 for example... in the case it is needed. |
| =Round(53,13.65)   | 54.6   | Rounds to the nearest multiple of 13.65.  We know, it's not very useful, but anyway, you can do it. |
| =Round(12.1,1/16)  | 12.25  | Rounds to the nearest 1/16. Useful when working with inches. |
| =Round(17,10,5)    | 15     | Rounds to the nearest 10 with a offset of 5.  In this example, 17 is rounded between 15 (10 with a 5 offset) and 25 (20 with a 5 offset), which returns 15. |
| =Round(12.3,1,0.5) | 12.5   | Rounds to the nearest integer with a offset of 0.5.  In this example, 12.3 is rounded between 11.5 (11 with a 0.5 offset) and 12.5 (12 with a 0.5 offset), which returns 12.5. |



## Algebra

### Sin

### Cos

### Tan

### Degree

### Radians

## Text 

### Replace

#### Description

The Replace function searches a text string for and specific text and replace it by another text.

#### Syntax

```
=Replace(text_to_modify, text_to_find, new_text, [start_occurrence], [nb_occurrences])
```

| Arguments        | Req/Opt  | Description                                                  |
| ---------------- | -------- | ------------------------------------------------------------ |
| text_to_modify   | Required | Text in which you want to replace some characters.           |
| text_to_find     | Required | Text to find and replace                                     |
| new_text         | Required | The text that will replace the characters in the text_to_find |
| start_occurrence | Optional | Specify at which occurrence of the text_to_find to start to replace it. |
| nb_occurrences   | Optional | Specify how many occurrences of the                          |

#### Examples

##### Example 1 - Simple replace

Replace all occurrences of a text into a text.

```
=Replace("My son have a son and my grandson have two sons", "son", "mother")
```

Result : "My mother have a mother and my grandmother have two mothers"