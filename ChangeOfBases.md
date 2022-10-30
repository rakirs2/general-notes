# Change Of Base

## Decimal
A little history. Way back when, in the early days of math... India finalized 2 very, very important contributions. The first was the concept of 0. The word in sanskrit in hindi is "Shunya" The second is the concept of base 10 or the modern decimal system.

Essentially, what this mean was that every number that we write has 10 options (0-9)

A little bit further down, we say we can BASE every number in 10. This was really easy for society to understand and math grew.

## Mathematicians are silly

Mathematicians like proving things completely. So eventually they asked themselves, "does math work regardless of base and can they be converted."

## Example

So lets start with a simple number 123. 

There are 123 units in here. However each position represents something different.

| 1     | 2    | 3    |
|-------|------|------|
| 10^2  | 10^1 | 10^0 |
| 100   | 10   | 1    |
| 100*1 | 10*2 | 3*1  |

To change base, we are effectively replacint the 10 with any counting number greater than 1

The most common are called binary (base 2) and hexadecimal (base 16)

So if were were to change 123 into base 2, what would we do?

| 1      | 1     | 1     | 1    | 0   | 1   | 1   |
|--------|-------|-------|------|-----|-----|-----|
| 2^6    | 2^5   | 2^4   | 2^3  | 2^2 | 2^1 | 2^0 |
| 64     | 32    | 16    | 8    | 4   | 2   | 1   |
| 123-64 | 59-32 | 27-16 | 11-8 | 3-0 | 3-2 | 1-1 |
