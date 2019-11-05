# Q0: Why are these two errors being thrown?

First error: We have some migrations that are yet to be run, meaning our schema is not yet up to date.
Second error: We haven't declared pokemon model yet, so it it not known to the controller.

# Q1: How are the random Pokemon appearing? What is the common factor between all the possible Pokemon that appear? *
They are all appearing on the top left page. And they are all small, basic pokemons that haven't evolved yet.

# Question 2a: What does the following line do "<%= button_to "Throw a Pokeball!", capture_path(id: @pokemon), :class => "button medium", :method => :patch %>"? Be specific about what "capture_path(id: @pokemon)" is doing. If you're having trouble, look at the Help section in the README.
When we click on the button "Throw a Pokeball!", it directs us to the path with prefix "capture", with the parameter set to @pokemon, and then apply a HTTP patch request.

# Question 3: What would you name your own Pokemon?
Asskicker

# Question 4: What did you pass into the redirect_to? If it is a path, what did that path need? If it is not a path, why is it okay not to have a path here?
It is a path. And it needs the prefix name of the path, telling it which path it should go to, and the parameter needed to navigate to that path.

# Question 5: Explain how putting this line "flash[:error] = @pokemon.errors.full_messages.to_sentence" shows error messages on your form.
errors.full_messages returns an array of all the error messages which is why you see the brackets and quotes. You can use .to_sentence to turn that array into a readable sentence.

# Give us feedback on the project and decal below!

# Extra credit: Link your Heroku deployed app
