# isat-subtask2

## Explanation of the Functions and Menu System

This program is a number converter that allows the user to convert numbers between decimal, binary, and hexadecimal formats. It uses four functions to keep the program organised and easy to understand.

The `decimalToBinary` function receives a decimal number and converts it to binary. It repeatedly divides the number by 2 and stores the remainders until the number becomes 0.

The `binaryToDecimal` function receives a binary number as text. It reads each digit, checks that it is either 0 or 1, and calculates the decimal value. If another digit is entered, the program displays an invalid binary message.

The `decimalToHexadecimal` function converts a decimal number to hexadecimal. It divides the number by 16 and uses the remainder to select the correct hexadecimal digit from 0 to 9 or A to F.

The `hexadecimalToDecimal` function converts hexadecimal input to decimal. It accepts digits from 0 to 9 and letters from A to F. Lowercase letters are also accepted because the program converts them to uppercase before calculating the answer.

The menu system displays six options. The user can choose a conversion option, run a demo, or exit the program. The menu repeats after each option, allowing the user to perform more conversions without restarting the program. The program only closes when option 6 is selected. 

## Examples

Example 1: Decimal to Binary

- Input: `25`
- Output: `11001` 

Example 2: Binary to Decimal

- Input: `1010`
- Output: `10`

Example 3: Decimal to Hexadecimal

- Input: `255`
- Output: `FF`

Example 4: Hexadecimal to Decimal

- Input: `1A`
- Output: `26`

Example 5: Demo Option

- The program generates a random number between 0 and 99.
- For example, if it generates `42`, the program displays `101010` as the binary value.

## Challenges Encountered During Modification

One challenge was understanding how each number system works. Binary uses base 2, while hexadecimal uses base 16. I solved this by using division and remainder operations in the conversion functions.

Another challenge was validating user input. A binary number must only contain 0 and 1, and a hexadecimal number must only contain digits from 0 to 9 and letters from A to F. I added checks so that the program displays an error message when invalid input is entered.

I also had to make sure that the menu repeats correctly after each conversion. This was solved by using a loop that continues until the user selects the Exit option.
