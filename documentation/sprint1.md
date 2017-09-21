html
    id: altitude
    id: fuel
    type: div
    purpose: to display the stuff)
    
    handlers
        args: none
        return: undefined
        behavior: listens to events and triggers controller
        purpose: to call controller method

    controller
        init: function
            args: 
            return: undefined
            behavior: get f/a data and call model to render
            purpose: get data and draw it

    model
        properties: 2
            fuel: number
                init: 1000
            altitude: number
                init: 0
        methods: 2 
            get_fuel:
                args: none
                return: number
                behavior: returns the stored fuel value
            get_altitude:
                args: none
                return: number
                behavior: returns the stored altitude value
    view
        draw fuel, altitude