# Cryptography---Pseudorandom-Number-Generation

# AIM:

To implement and demonstrate pseudorandom number generation using the standard library.

## DESIGN STEPS:

### Step 1:

Understand the concept of pseudorandom number generation (PRNG).

### Step 2:

Implement the pseudorandom number generation using a programming language and its standard library functions.

### Step 3:

In PRNG, random numbers are generated based on an initial seed value, and the sequence of random numbers follows a deterministic process.
Many programming languages provide built-in functions for generating pseudorandom numbers, such as random() in Python and rand() in C.
These numbers are uniformly distributed within a given range and can be used in various applications such as cryptography, simulations, and games.

The pseudorandom number generation can be represented as:
𝑋𝑛 + 1 = (𝑎𝑋𝑛 + 𝑐) mod 𝑚 where 𝑎, 𝑐, and 𝑚 are constants and 𝑋𝑛 is the nth number in the sequence.

## PROGRAM:

~~~
#include <stdio.h>
#include <stdlib.h>
#include <time.h>

// Function to generate a random integer
void generate_random_numbers()
{
    printf("Random integer: %d\n", rand());
}

int main()
{
    // Seed the random number generator with the current time
    srand(time(0));
    
    // Generate random numbers
    generate_random_numbers();
    
    return 0;
}
~~~

## OUTPUT:

![image](https://github.com/user-attachments/assets/6990ff54-d8f0-49f3-a2ba-9b9a4bc95f05)

## RESULT:

The program is executed successfully, demonstrating pseudorandom number generation using the standard library functions in C.
