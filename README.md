A kata on implementing addition using Roman numerals; shamelessly plagiarised from Woody Zuill...

# Roman Addition

The Roman system for counting used the letters I, V, X, L, C, D and M to represent the Arabic numeric values 1, 5, 10, 50, 100, 500 and 1,000 respectively.  Note 5 cannot be represented by IIIII, etc.

The number 1 was represented by I, 2 by II, 3 by III.  But 4 was a special case represented by IV.  Likewise, 9 was represented by IX, 14 by XIV and 19 by XIX.  Similar combinations were used for 40 (XL), 90 (XC), 400 (CD) and 900 (CM).  Using this representation 499 and 949 are written as CDXCIX and CMXLIX respectively.

Here are some other examples:

```
1990 -> "MCMXC" (1000 -> "M"  + 900 -> "CM" + 90 -> "XC")
2008 -> "MMVIII" (2000 -> "MM" + 8 -> "VIII")
99 -> "XCIX" (90 -> "XC" + 9 -> "IX")
47 -> "XLVII" (40 -> "XL" + 7 -> "VII")
```
Your job, as mandated by Claudia Arithemeticus, the eminent Roman mathematician, is to write a program that can handle Roman addition.

You may implement the program in a programming language of your choice, but Claudia has however set some constraints based on advice from the software engineer Robertus Martinus:

* you should avoid using a case/switch statement
* you should not take, return, nor employ in the calculation any numeric literals
* you must demonstrate that your program works
* you should use a test driven development (TDD) approach to develop your program

To get you started, here are some examples of Roman addition that Claudia has written down for you:

```
I + I = II
I + II = III
II + I = III
II + II = IV
III + I = IV
IV + I = V
III + II = V
III + III = VI
I + VI = VII
VI + II = VIII
VI + III = IX
VIII + I = IX
IV + V = IX
V + V = X
VI + VI = XII
X + X = XX
XLV + V = L
XXXV + V = XL
XXXV + VI = XLI
XXV + XXV = L
```

Finally, a more extensive list of digits follows:

```
"I" -> 1
"II" -> 2
"III" -> 3
"IV" -> 4
"V" -> 5
"VI" -> 6
"VII" -> 7
"VIII" -> 8
"IX" -> 9

"X" -> 10
"XX" -> 20
"XXX" -> 30
"XL" -> 40
"L" -> 50
"LX" -> 60
"LXX" -> 70
"LXXX" -> 80
"XC" -> 90

"C" -> 100
"CC" -> 200
"CCC" -> 300
"CD" -> 400
"D" -> 500
"DC" -> 600
"DCC" -> 700
"DCCC" -> 800
"CM" -> 900

"M" -> 1000
"MM" -> 2000
"MMM" -> 3000
"MMMM" -> 4000
```
