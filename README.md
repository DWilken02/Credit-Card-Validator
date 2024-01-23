# _Credit Card Validator_

#### By _**DWilken02**_

#### _A program that checks if a credit card is valid_

## Technologies Used

* _HTML_
* _CSS_
* _JavaScript_

## Description

_A program that checks if a credit card is valid_

## Setup/Installation Requirements

1. Click the green code button
2. Then click download zip
3. Open the project folder
4. Then drag the index.html file to a browser of your choice

## Tests: 

Describe: passesLuhnAlgorithm();

Test 1: "Should return true if the number given passes Luhn Algorithm"
Code: passesLuhnAlgorithm("4102080860435620");
Expected output: True 

## Known Bugs

* _No known Bugs_

## License

_[MIT](LICENSE.txt)_

Copyright (c) _2024_ _DWilken02_

## Breaking down the problem

1. Apply Luhn Algorithm
  * Take in the credit card number
  * Double every other number from right to left
  * For every doubled digit that becomes a double digit number add together each digit of the double digit number. 
  * Add all the digits in the transformed number together to get the sum.
  * Check if number is valid. Valid numbers end in 0. If valid then return True. If not then return false.

2. Validate length of number
  * Take in Credit Card Number.
  * If the first digit is 4 and the length is 16 then it belongs to Visa.
  * If the first digit is 5 and the length is 16 then it belongs to MasterCard.
  * If the first digit is 6 and the length is 16 then it belongs to Discover.
  * If the first 2 digits are 34 or 37 and the length is 15 then it belongs to American Express.
  * If the number does meet any of the above rules return true. If not then return false.

3. If any of the above rules are false return "This card number is not valid." Otherwise return "This card number is valid."