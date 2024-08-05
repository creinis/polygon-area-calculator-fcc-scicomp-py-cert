# Shape Calculator

###### Technologies:
<p align="center">
<img src="https://img.icons8.com/color/75/000000/python.png" width="75" height="75" alt="Python" style="margin: 10px 15px 0 15px;" />
</p>

### Try it!

To run the Shape Calculator application, follow the instructions in the Setup section below.

## Project Structure

- `shape_calculator.py`: Contains the implementation of the `Rectangle` and `Square` classes.

## Setup

### Prerequisites

- Python 3 installed

### Installation Steps

1. Clone the repository:
   ```bash
   git clone https://github.com/creinis/polygon-area-calculator-fcc-scicomp-py-cert.git
   cd shape-calculator-fcc-scicomp-py-cert
   ```

2. Run the Shape Calculator script:
   ```bash
   python3 main.py
   ```

## Shape Calculator

### Functionality

The Shape Calculator allows you to create and manipulate `Rectangle` and `Square` objects. It provides methods to calculate area, perimeter, and diagonal, as well as to represent the shapes visually with asterisks.

### Rectangle Class

#### Methods

- `__init__(self, width, height)`: Initializes a new rectangle with a given width and height.
- `set_width(self, width)`: Sets the width of the rectangle.
- `set_height(self, height)`: Sets the height of the rectangle.
- `get_area(self)`: Returns the area of the rectangle.
- `get_perimeter(self)`: Returns the perimeter of the rectangle.
- `get_diagonal(self)`: Returns the diagonal of the rectangle.
- `get_picture(self)`: Returns a string representation of the rectangle using asterisks, or a message if the rectangle is too large.
- `get_amount_inside(self, shape)`: Returns the number of times the given shape can fit inside the rectangle.
- `__str__(self)`: Returns a string representation of the rectangle.

### Square Class

#### Methods

The `Square` class inherits from the `Rectangle` class and overrides the following methods:

- `__init__(self, side)`: Initializes a new square with a given side length.
- `set_side(self, side)`: Sets the side length of the square.
- `__str__(self)`: Returns a string representation of the square.
- `set_width(self, width)`: Sets the width (and height) of the square.
- `set_height(self, height)`: Sets the height (and width) of the square.

### Practical Use Case

The Shape Calculator is useful for performing geometric calculations and visualizing shapes. It can be used in various applications, such as graphic design, architecture, and education.

### Benefits

- **Ease of Use:** Provides simple methods to manipulate and visualize shapes.
- **Flexibility:** Supports both rectangles and squares, allowing for versatile use cases.
- **Python Standard Library:** Utilizes Python’s built-in data structures for implementation.

## How to Use

1. Create instances of the `Rectangle` and `Square` classes.
2. Use the methods to calculate properties and visualize the shapes.

### Example Usage

```python
import shape_calculator

rect = shape_calculator.Rectangle(5, 10)
print(rect.get_area())          # Output: 50
rect.set_width(3)
print(rect.get_perimeter())     # Output: 26
print(rect)                     # Output: Rectangle(width=3, height=10)

sq = shape_calculator.Square(9)
print(sq.get_area())            # Output: 81
sq.set_side(4)
print(sq.get_diagonal())        # Output: 5.656854249492381
print(sq)                       # Output: Square(side=4)
```

### Example Output

```plaintext
50
26
Rectangle(width=3, height=10)
81
5.656854249492381
Square(side=4)
...............
----------------------------------------------------------------------
Ran 15 tests in 0.001s

OK
```

### Additional Information

- **Shape Representation:** Visualizes shapes using asterisks, making it easier to understand their structure.
- **Geometric Calculations:** Provides essential methods for calculating area, perimeter, and diagonal.

---
#### This is a FreeCodeCamp Challenge for Scientific Computing with Python Projects Certification.
<p align="center">
<img src="https://cdn.freecodecamp.org/platform/universal/fcc_primary.svg" width="250" height="75" alt="freeCodeCamp" style="margin: 0 15px; opacity: 0.6" />
</p>
