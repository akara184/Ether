
# SOME RANDOM THOUGHTS ABOUT 

### C++ and C, difference of `&` and `*`

- `&` -> "the address of"
- `*` -> "what's at"

```cpp
int x;    // Declares x as having type int.
int y;    // Declares y as having type int.
int *p;   // Declares *p as having type int, which means that p has type pointer-to-int.

p = &x;   // Uses & to get a pointer to x, and stores it in p. p now contains the value &x.
// We say that "p points to x". In other words, *p is x.
x = 10;   // Sets the value of the variable x to be 10.
y = *p;   // Gets the value 10 from x through the pointer p and stores in y. y is now 10.
*p = 42;  // x is now 42, and y is still 10.
p = &y;   // Set p to point to y instead. *p is now y.
x = *p;   // x is now 10 again.
