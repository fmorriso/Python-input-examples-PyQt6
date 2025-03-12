# Python Input Examples (PyQT6)
Example of input() encapsulated in a library (InputUtilities class) that uses the PyQT6 package for the GUI.

All the methods are static, so you do not need to create an instance of the class to use its methods.

## Example usage
To use the input utilities (InputUtils class) and its static methods:
### Yes/No questions examples
<pre> 
from input_utilities import InputUtils as IU

yn: bool = IU.get_yesno_response('Fast Food Order','Do you want ketchup?')
</pre>

### Whole number input examples

<pre> 
from input_utilities import InputUtils as IU

n: int = IU.get_whole_number('Restaurant', 'How many people are in your party? ')
n: int = IU.get_whole_number_in_range('Restaurant','How many people are in your party? ', 1, 7)
</pre>

### Floating point number input examples

<pre> 
from input_utilities import InputUtils as IU

x: float = IU.get_floating_point_number('Apples Purchase', 'What was the weight in pounds? ')
x: float = IU.get_floating_point_number_in_range('Fuel', 'How many gallons do you wish to purchase? ', 0.5, 22.5)
</pre>

### Decimal number input examples

<pre> 
import decimal
from decimal import Decimal
from input_utilities import InputUtils as IU

d: decimal = IU.get_decimal_number('ATM', 'How much money do you wish to withdraw? ')
d: decimal = IU.get_decimal_number_in_range('ATM', 'How much money do you wish to withdraw? ', 5, 600)
</pre>

## Tools Used

| Tool     |  Version |
|:---------|---------:|
| Python   |   3.13.2 |
| PyQt6 |    6.8.1 |
| PyCharm  | 2024.3.4 |
| VSCode   |   1.98.0 |

## Change History

| Date       | Description      |
|:-----------|:-----------------|
| 2025-03-11 | Initial creation |

## References

* [Python decimal type](https://docs.python.org/3/library/decimal.html)