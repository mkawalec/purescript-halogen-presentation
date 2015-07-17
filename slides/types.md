##  Types

arrays are single-type JS arrays

polymorphic type annotations need explicit forall

    identity :: forall a. a -> a
    identity x = x

row polymorphism, accepts any object conforming to spec

    addProps :: forall r. { foo: Number, bar :: Number | r } -> Number
    addProps o = o.foo + o.bar

