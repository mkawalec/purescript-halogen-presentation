##  Handling user events

    ui :: Signal Input -> Signal (HTML Input)
    ui future = render <$> stateful update 0 future
    where
        render count =
            button [ onClick \_ -> ButtonClicked ]
                   [ text (show count) ]
