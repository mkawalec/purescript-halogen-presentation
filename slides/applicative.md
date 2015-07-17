##  Applicative

    (<$>) :: (a -> b) -> Signal a -> Signal b
    (<*>) :: Signal (a -> b) -> Signal a -> Signal b

So we can have

    type InputState = { firing :: Bolean, direction :: Point }

    inputState :: Signal InputState
    inputState = { firing: _, direction: _ }
                    <$> keyPressed Space
                    <*> mousePosition
