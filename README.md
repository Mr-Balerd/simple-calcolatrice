# Engineering Calculator (C++)

A menu-driven command-line engineering calculator built with **C++17**. It is designed as a beginner-to-intermediate portfolio project and demonstrates functions, input validation, loops, vectors, algorithms, and numerical calculations.

## Features

- **Basic arithmetic:** addition, subtraction, multiplication, division, and powers
- **Scientific functions:** trigonometry, inverse trigonometry, square root, natural/base-10 logarithms, factorial, absolute value, and angle conversion
- **Unit conversions:** temperature, speed, length, mass, and pressure
- **Statistics:** count, sum, mean, median, minimum, maximum, population variance, and standard deviation
- **Quadratic equations:** real, repeated, and complex roots; handles linear and degenerate cases
- **Ohm's law:** calculate voltage, current, or resistance
- **Input validation:** checks invalid input and common mathematical domain errors

## Requirements

- A C++17-compatible compiler (GCC, Clang, or MSVC)
- CMake 3.16+ (optional, but recommended)

## Build and run

### Option 1: Compile directly

**GCC / Clang**
```bash
g++ -std=c++17 -Wall -Wextra -Wpedantic src/main.cpp -o engineering_calculator
./engineering_calculator
```

**Windows (MinGW)**
```bash
g++ -std=c++17 -Wall -Wextra -Wpedantic src/main.cpp -o engineering_calculator.exe
engineering_calculator.exe
```

### Option 2: CMake

```bash
cmake -S . -B build
cmake --build build
```

Run the generated executable from the build directory (the exact path depends on your operating system and generator).

## Notes

- Trigonometric input is interpreted in **degrees**; inverse trigonometric results are returned in degrees.
- Variance and standard deviation are calculated for the full supplied dataset (population formulas).
- Factorial accepts integer values from 0 to 170, which is the practical range for a `double` result.
- Floating-point calculations have finite precision. Results are intended for learning and general calculations, not safety-critical engineering design.

## Project structure

```text
engineering-calculator-cpp/
├── src/
│   └── main.cpp
├── CMakeLists.txt
├── .gitignore
└── README.md
```

## Possible future improvements

- Add matrix operations and complex-number support
- Add unit tests with CTest
- Add a graphical user interface
- Support configurable precision and calculation history

## License

This project is released under the MIT License. See [LICENSE](LICENSE).
