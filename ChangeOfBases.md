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


So now you have a general idea. Essentially you take the largest power continually subtract values.

### More worked example
Let's look at base 16 step by step

Again, same number 123

First I ask myself, what's the largest power of 16 that's less than 123.

16^0 = 1
16^1 = 16
16^2 = 256

256 is definitely more than 123. So I'm going to say, how many 16s go into 123

```
123/16 = 7 R 11
```

We have 11 remaining. So now I want to go to the next value down which is 16^0. 16^0 = 1. THere are 11 left. So The value for that "spot" is 11.

So the representation looks something like this

| 0     | 7        | 11    |
|-------|----------|-------|
| 16^2  | 16^1     | 16^0  |
| 0     | 7        | 11    |
| 123-0 | 123-16*7 | 11-11 |


Now, again, in base 10, haveing a number > 9 in any spot does not make any sense. But we can think of it as:

7*16^1 + 11*16^0 = 123 in base 10

Now, there's a little trick in computer science. We call base 16 "hexadecimal" hexa meaning 6, decimal meaning 10. The numbers in decimals go 

```
0,1,2,3,4,5,6,7,8,9
```

In hexadecimal, they go 
```
0,1,2,3,4,5,6,7,8,9,a,b,c,d,e,f
```

So 123 in hexadecimal is 7b

If you want to change this/play with it, here are a few more resources:

* https://www.khanacademy.org/math/algebra-home/alg-intro-to-algebra/algebra-alternate-number-bases/v/number-systems-introduction
* https://www.rapidtables.com/convert/number/base-converter.html
