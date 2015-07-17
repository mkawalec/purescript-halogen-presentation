##  Composing signals

We can map functions over signals

    (<$>) :: (a -> b) -> Signal a -> Signal b

For example

    x :: Signal Number
    x = _.x <$> mousePosition
