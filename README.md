# Blog-Generator
A simple blog generator using OpenAI

I will atempt to explain the program using little to no technical terms.
The first four lines of code are asking permission to OpenAI to use their API. This is done by purchasing an API key that allows us to use their services.
Once we have this key, everytime the code runs, OpenAI will check that we have a valid key, if we do, then we are allowed to use whatever services we purchased.
After we are granted accesss to the services, we create a function that will generate the blog response based on some given topic.
Inside the function, we create a completion called response that will generate our prompt response. Inside the completion, we have a variable called 'model' in which
we specify the type of machine learning model we will use to generate our response.
We then specify a 'prompt'. Note that this is not the prompt that the user will enter. This prompt is to tell the machine learning what we want it to do with the user's
prompt. In this case, we ask the model to write a paragraph about the topic the user entered.
We then decide how long the response will be based on a number of 'tokens'. This tokens are what we purchased from OpenAI.
Finally, we specify how random our response will be, using a variable called, 'temperature', that ranges from 0 to 1 with values closer to 0 as being more well-defined
responses and values closer to 1 as being more creative.
