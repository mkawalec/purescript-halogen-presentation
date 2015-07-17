##  DOM Templating

There is a DOM templating DSL

    ui = div [ className "wrapper" ]
             [ h1_ [ text "Hello world!" ]
             , p [ text "An example" ]
             ]
