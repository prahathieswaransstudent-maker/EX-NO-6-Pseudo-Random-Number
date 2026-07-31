# EX-NO-6: Pseudo-Random Number Generation

## AIM
To implement pseudorandom number generation using the standard C library.

## ALGORITHM
1. Start the program.
2. Import the required header files.
3. Seed the random number generator using the current time (`srand(time(0));`).
4. Read the number of random numbers to generate.
5. Generate random numbers using `rand()` inside a loop.
6. Display the generated random numbers.
7. End the program.

## PROGRAM

```c
#include <stdio.h>
#include <stdlib.h>
#include <time.h>

int main()
{
    int n, i;

    // Seed the random number generator
    srand(time(0));

    printf("Enter the number of random numbers to generate: ");
    scanf("%d", &n);

    printf("Generated Random Numbers:\n");

    for(i = 0; i < n; i++)
    {
        printf("%d\n", rand());
    }

    return 0;
}
```

## SAMPLE OUTPUT

```
Enter the number of random numbers to generate: 5
Generated Random Numbers:
1804289383
846930886
1681692777
1714636915
1957747793
```

> **Note:** The output values will be different each time the program is executed because the random number generator is seeded using the current system time.

## RESULT
Thus, the program for pseudorandom number generation using the standard C library was implemented and executed successfully.
