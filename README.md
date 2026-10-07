# CIS-165 Lab 2

Course section: CIS-165-W198

## Initial Plans

### Program 1 — Sum of Two Numbers

I will store 50 and 100 in two integer variables. I will add the two variables together and store the result in a variable named `total`. Then I will display the value of `total` with a clear label.

### Program 2 — Miles Per Gallon

I will store 312 miles and 16 gallons in variables. I will divide the miles by the gallons and store the result in an `mpg` variable. I will use `double` so the calculation can keep a fractional result. Then I will display the MPG result with its units.

## How to Run

### sum.cpp

Compile the program with:

    g++ -std=c++17 -Wall -Wextra sum.cpp -o sum

Run the program with:

    ./sum

### mpg.cpp

Compile the program with:

    g++ -std=c++17 -Wall -Wextra mpg.cpp -o mpg

Run the program with:

    ./mpg

The programs can also be opened and run separately in an online C++ compiler such as OnlineGDB.

## Testing

Before each test, I calculated the expected result myself. I then ran the program and compared the actual output with the expected result.

| Program                  | Values used              | Expected result | Actual output                  | Match or fix |
| ------------------------ | ------------------------ | --------------- | ------------------------------ | ------------ |
| sum.cpp — assigned values | 50 and 100               | 150             | Total: 150                     | Match        |
| sum.cpp — changed values  | 25 and 75                | 100             | Total: 100                     | Match        |
| mpg.cpp — assigned values | 312 miles; 16 gallons    | 19.5 MPG        | Miles per gallon: 19.5 MPG    | Match        |
| mpg.cpp — changed values  | 250 miles; 12 gallons    | 20.8333 MPG     | Miles per gallon: 20.8333 MPG | Match        |

After completing the changed-value tests, I restored the originally assigned values in both source files and reran the programs.

## Code Explanations

### sum.cpp

The program stores 50 in one variable and 100 in another variable. The two values are added together and the result is stored in `total`. The program then displays `total`. Storing the calculation in `total` before printing keeps the calculation separate from the output and makes it clear what the resulting value is.

### mpg.cpp

The miles-per-gallon formula is miles divided by gallons. The program stores 312 miles and 16 gallons and divides them to get 19.5 MPG. I used `double` for the variables so the result can contain a decimal. If two integer operands are divided in C++, integer division is performed and the fractional part is discarded. In the changed-value test, 250 miles divided by 12 gallons produced approximately 20.8333 MPG. The result was stored in `mpg` before being displayed.
