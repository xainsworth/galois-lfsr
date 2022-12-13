# galois-lfsr
A 2^n bit keystream generator with random Galois LFSR and Boolean Functions

## What is Galois LFSR
A Galois linear feedback shift register (LFSR) is a type of shift register that uses feedback to generate a sequence of pseudorandom numbers. It works by taking a series of bits and shifting them to the right by one position, with the first bit being replaced by the result of a bitwise exclusive-or operation performed on some or all of the bits in the register. This process is repeated, with the resulting sequence of bits being used as the input to the exclusive-or operation. This allows the LFSR to generate a sequence of numbers that appears random, but is actually completely determined by the initial state of the register and the feedback function used.

## How do we know which bits are we going to use exclusive-or operation with?
In a Galois LFSR, the bits that are used in the exclusive-or operation are determined by the feedback function. This function is typically defined as a polynomial over the field of binary numbers, with the coefficients of the polynomial corresponding to the bits that are used in the exclusive-or operation. For example, if the feedback function is x^3 + x + 1, this would mean that the first, third, and fourth bits in the register are used in the exclusive-or operation.
