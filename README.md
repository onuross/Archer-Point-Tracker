# Archer Point Tracker

This Python script is an archery competition point tracker that allows users to input and analyze the performance of multiple archers across various shots. It includes features such as:

- User input validation for the number of archers and shots.
- Creation of a point table displaying the distribution of points for each archer.
- Wind conditions tracking, with a dedicated table showing the missed shot rate based on wind conditions.
- Calculation of the percentage of points achieved by all archers across different point categories.

## Usage

1. Run the script and input the number of archers and shots as prompted.
2. Enter the points achieved by each archer for each shot.
3. Provide wind conditions for missed shots when prompted.
4. The script will generate a point table, a wind condition table, and the percentage of points for all archers.

## Code Overview

The script is organized into several functions:

- `numberArcher()` and `numberShot()`: Input functions ensuring the correct number of archers and shots.
- `listMaker()`: Creates a two-dimensional point list for the point table.
- `statistics()`: Fills up the point list based on user input and tracks wind conditions.
- `pointTableWrite()`: Prints the point table with archer-wise point distribution.
- `windController()` and `windTableWrite()`: Manage and display wind conditions and missed shot rates.
- `allArchersPer()`: Calculates and prints the percentage of points achieved by all archers.

## Sample Output

Running the script will generate output similar to:

```plaintext
Archer Reg No    10p    9p     8p     7p     6p     5p     4p     3p     2p     1p     0p    Total
-------------   ----   ----   ----   ----   ----   ----   ----   ----   ----   ----   ----   -----
1              3      2      1      0      1      2      3      4      5      6      7      36    
2              4      3      2      1      0      1      2      3      4      5      6      36    
...
All Archers(%)  10.00  9.00   8.00   7.00   6.00   5.00   4.00   3.00   2.00   1.00   0.00
