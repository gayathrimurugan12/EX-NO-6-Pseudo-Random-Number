# EX-NO-6-Pseudo-Random-Number

# AIM: 
Implementation of Pseudorandom Number Generation Using Standard library

# ALGORITHM:
Start the program and import the required libraries.
Seed the random number generator using the current time(i.e) rand(time(0));
Get the number of randon number to generate.
Pass the value for number of iterations and print the numbers.
End the program.

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
    int n, i;
    printf("\n\n\n\n    *****Pseudorandom number generator*****\n\n\n\n");
    printf("Enter the seed value: ");
    scanf("%u", &seed);
    printf("Enter how many random numbers to generate: ");
    scanf("%d", &n);
    printf("Random numbers:\n");
    for (i = 0; i < n; i++) {
        seed = lcg(seed);
        printf("%u\n", seed);
    }
    return 0;
}

```


# OUTPUT:


![Screenshot 2025-04-07 160345](https://github.com/user-attachments/assets/fea56012-54ef-4106-ab96-c4cbdd777f75)


# RESULT:
The program to generate pseudorandom number executed successfully.
