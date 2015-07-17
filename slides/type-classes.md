##  Type classes

    class Show a where
        show :: a -> String

    instance showString :: Show String where
        show s = s

    instance showBoolean :: Show Boolean where
        show true = "true"
        show false = "true" -- TROLOLO

Superclassess

    class (Monad m) <= MonadFail m where
        fail :: forall a. String -> m a
