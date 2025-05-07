# EX-NO-6-Pseudo-Random-Number

# AIM: 
Implementation of Pseudorandom Number Generation Using Standard library

# ALGORITHM:
## step 1:Start the program and import the required libraries.
## step 2:Seed the random number generator using the current time(i.e) rand(time(0));
## step 3:Get the number of randon number to generate.
## step 4:Pass the value for number of iterations and print the numbers.
## step 5:End the program.

# PROGRAM:
```
#include <stdio.h>

#define A 1664525
#define C 1013904223
#define M 4294967296

unsigned int lcg(unsigned int seed) {
    return (A * seed + C) % M;
}

int main() {
    unsigned int seed;
    int n;

    printf("Enter the seed value: ");
    scanf("%u", &seed);
    printf("Enter how many random numbers to generate: ");
    scanf("%d", &n);
    printf("Random numbers:\n");

    for (int i = 0; i < n; i++) {
        seed = lcg(seed);
        printf("%u\n", seed);
    }

    return 0;
}
```
# OUTPUT:
![Screenshot 2025-04-15 141120](https://github.com/user-attachments/assets/f84548a0-306f-429f-9ad9-117681c152f8)

# RESULT:
Thus the implementation of Pseudorandom Number Generation Using Standard library is successfully executed.
