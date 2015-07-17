##  Types continued

RankNTypes is included by default

    poly :: (forall a. a -> a) -> Boolean
    poly f = (f 0 < 1) == f true

Type synonyms are supported

    type Foo = { foo :: Number, bar :: Number }

    addFoo :: Foo -> Number
    addFoo = \o -> o.foo + o.bar
