##  Signals

Values that change over time:

    type Signal a = Time -> a

Examples:

    mousePosition :: Signal Point
    keyPressed :: Key -> Signal Boolean
