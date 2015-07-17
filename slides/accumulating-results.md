##  Accumulating Results

We can accumulate a result in response to a signal:

    stateful :: s ->
                (s -> i -> s) ->
                Signal i ->
                Signal s

For example

    combine :: (Monoid a) => Signal a -> Signal a
    combine = stateful mempty (<>)
