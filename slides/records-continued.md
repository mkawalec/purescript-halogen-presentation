##  Records, continued

Records can be extensible:

    type Lang l = { language :: String | l }
    type Language = Lang ( country :: String )

Update syntax is Haskell-like:

    setX :: Number -> Point -> Point
    setX val point = point { x = val }

