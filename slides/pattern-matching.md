##  Pattern matching

Like in haskell:

    f [x] = x
    f [x, y] = x / y
    f _ = 0

    data Foo = Foo String | Bar Number Boolean

    foo (Foo s) = true
    foo (Bar _ b) = b

And we have guards:

    sth [] = 0
    sth (x:xs) | x % 2 == 0 = 1 + sth xs
    sth (_:xs) = sth xs

