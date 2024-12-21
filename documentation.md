# Lune Documentation

## Structure
Tabs in Lune can be any length, so:
```lune
for(var i = 1, i <= 10, i++) {
    print(i)
}
```
is the same as:
```lune
for(var i = 1, i <= 10, i++) {
  print(i)
}
```

In fact, most whitespace in Lune is ignored, so you can also have random tab lengths,
```lune
      for(var i = 1, i <= 10, i++) {
         print(i)
}
```
negative tab lengths,
```lune
  for(var i = 1, i <= 10, i++) {
print(i)
  }
```
or... whatever the actual heck this is.
```lune
for(var i


           = 1, i <=
                      10, i++
   ) {print(

i)}
```

To write comments, precede them with `//`...
```lune
// This is a comment
```
...or start them with `/*` and end them with `*/`.
```lune
/* This is a
comment */
```

The `...` keyword appears a lot in this documentation, and acts as a no-op.

## I/O
To print text to the console, use the `print` command.
```lune
print("Hello!")
```

Asking the user a question can be done with the `ask` command set.
```lune
asknum("How many pets do you have?")
askstr("What's your name?")
askbool("Are you right-handed?")
askoptions("What's your favorite color?", ["Red", "Blue", "Yellow", ...])
```
Or if you just want to wait until the user presses a key, use the `getkey` command.
```lune
getkey()
```

## Variables
To define a variable, use `var`.
```lune
var i = 0
```
To make it unchangeable, use `const`.
```lune
const pi = 3.14
```
Modifying variables can be done like this:
```lune
i += 1
i -= 2
i *= 3
i /= 4
...
```
You can also do this one one-input functions.
```lune
i sin=

// I'm sorry
```

Lune *does* support local variables and garbage collection, but if you want to delete a variable you don't need anymore, use `delvar`.
```lune
delvar i
```

Giving a variable a specific type can be done with `: [type]` after the variable name.
```lune
var k: uint = 25
```

**List of built-in constants:**
```lune
PI // ~3.14
E // ~2.71
PHI // ~1.61
ROOT2 // ~1.41
ROOTHALF // ~0.70
INF // Infinity
NEGINF // Negative infinity
NaN // An illegal operation will return this
this // Refers to whatever is running the code
null // Absolutely nothing
```

**List of variable types:**
```lune
float // A number with a decimal place
unybble // An integer from 0 to 15
nybble // An integer from -8 to 7
ubyte // An integer from 0 to 255
byte // An integer from -128 to 127
uword // An integer from 0 to 65535
word // An integer from -32768 to 32767
uint // An integer from 0 to 4 billion
int // An integer from -2 billion to 2 billion
string // A letter, word, or line of text
boolean // True or false
function // A line of code or group of lines of code
array // A list of elements
object // A list of keys and values
any // Any of these
none // None of these
```

If you create a variable whose initial value is a number, its type will default to `float` of it has a decimal point, or `int` otherwise.

## Computations
**List of mathematical functions in Lune:**
```lune
a+b a-b a*b a/b a%b a**b
sqrt(a) cbrt(a) root(n, a)
log(a) log(b, a) ln(a)
constrain(n, lo, hi) abs(n)
sin(n) cos(n) tan(n)
asin(n) acos(n) atan(n)
atan2(x, y)
```

**List of logical and bitwise functions:**
```lune
a&&b a||b a^^b
!a a!&b a!|b a!^b
a&b a|b a^b ~a
```

**List of comparison predicates:**
```lune
a==b a<b a>b
a!=B a<=b a>=b
a===b
ternop(c, t, f) // similar to c?t:f
```

## Arrays
The `array` keyword will return a list with a given length. All its values will be null.
```lune
array(10)
```

## Objects
WIP

## Strings
WIP

## Randomization
WIP

## Control
WIP

## Debugging
WIP

## Other
WIP
