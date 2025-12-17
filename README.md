# Triangle Classification Unit Testing

## Overview
This project demonstrates **unit testing of a triangle classification function**.  
The function classifies triangles based on their side lengths into **Equilateral, Isosceles, or Scalene**, and handles invalid input cases.

The goal of this project is to ensure that the triangle classification function works correctly for **all valid and invalid inputs**, using **professional testing practices**.

---

## Triangle Classification Rules

A triangle can be classified based on its side lengths:

| Triangle Type   | Rule                                      |
|-----------------|-------------------------------------------|
| Equilateral     | All three sides are equal                 |
| Isosceles       | Any two sides are equal                   |
| Scalene         | All three sides are different            |

### Invalid Triangles
- Any side is zero or negative → **raises ValueError**
- Sum of any two sides ≤ third side → **raises ValueError**

---

## Test Scenarios
- Equilateral triangle
- Isosceles triangle
- Scalene triangle
- Zero or negative side length (ValueError expected)
- Triangle inequality violation (ValueError expected)
- Floating point sides (Equilateral, Isosceles, Scalene)
- Very large numbers
- Boundary values (barely valid triangles)
- Additional triangle inequality violation scenarios

---

## Example Usage of Tests

- **Equilateral:** `(5, 5, 5)` → Returns `"Equilateral"`  
- **Isosceles:** `(5, 5, 3)` → Returns `"Isosceles"`  
- **Scalene:** `(4, 5, 6)` → Returns `"Scalene"`  
- **Invalid input:** `(0, 4, 5)` or `(1, 2, 3)` → Raises `ValueError`  

> Each scenario has a corresponding test function in `test_triangle.py`.

---

## Notes
- `test_triangle.py` contains all **mandatory and additional professional test cases**.  
- Designed to validate the **triangle classification function thoroughly and professionally**.

## Project Structure

