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
