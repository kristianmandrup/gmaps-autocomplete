# Geocoding and autocomplete with Google Maps and jQuery UI

A simple demo showing how to use the jQuery UI autocomplete widget in conjunction with Google Maps geocoding service.

See it in action here: [rjshade.github.com/gmaps-autocomplete/](http://rjshade.github.com/gmaps-autocomplete/)

Some more explanation here: [rjshade.com/2012/03/30/Google-Maps-autocomplete-with-jQuery-UI](/[http://www.rjshade.com/2012/03/30/Google-Maps-autocomplete-with-jQuery-UI/)

## Use with Rails form helpers
I've had success using this with the [SimpleForm](https://github.com/plataformatec/simple_form) gem:

    = simple_form_for(@post) do |f|
        = f.input :address, :input_html =>{:id => 'gmaps-input-address'}, :placeholder => 'Start typing a place name...'
