# gpt_cli

This version is updated by Rowan Kelleher

Updated features:
1. Prompt to ask you what model you want to use
   1. Use "3.5" or "4" shortcuts to use "gpt-3.5-turbo" and "gpt-4"
   2. Or just type in the applicable name
2. Prompt asking you if you want to save your responses
   1. If you say "yes" then the program will log your model, prompt, and response in a different file for each day


https://github.com/zawawiAI/gpt_cli/assets/50743060/9dbbeeec-f2aa-43cc-bd05-80a2dfebba32




Notes: This is NOT ChatGPT since the ChatGPT API has not been released yet, but you can use OpenAI API with GPT-3 capability (https://beta.openai.com/docs/introduction).

However once ChatGPT API is made available to the public, I personally think you can just change the API Key with very little modification to the code or it requires no modification at all.


This scripts allows you to use OpenAI API in both your Linux and Windows terminals. 

This is a command line tool that allows you to search using the OpenAI API your CLIs such as Linux terminal or Windows Command Prompt. It uses the openai library to interact with the API and the text-davinci-003 model to generate responses to your queries.

Getting Started

Install the openai library by running `pip install openai` in your command line.

Set up an API key for the OpenAI API by signing up for an account on the OpenAI website and obtaining a key.

Replace "Your OpenAI API Key" in the code with your own API key.

Run the code with `python gpt_cli` (Linux and Windows) and start searching.

Usage

The tool will prompt you to enter a search query. Once you enter your query, it will generate a response using the text-davinci-003 model. You can search for any topic you want, and the model will generate a relevant response.

In gpt_cli.py I have added 3 new features

1)To save the previous response to a text file, input "save" and enter a file name when prompted.
2)To exit the script, input "exit".

3)Error Handling
The script includes error handling for the following exceptions:

openai.exceptions.OpenAiError
IndexError: when no response is generated
Exception: for any other errors that may occur.
Please reach out to OpenAI if you are facing any issues with the API.


You can change the model_engine to any other OpenAI's models. Also, you can play with the max_tokens, n, stop, and temperature parameters to customize the output of the model.

Tips

Keep your queries concise and specific for more accurate results.
If you are not satisfied with the response, try rephrasing your query or adjusting the temperature parameter.
Feel free to experiment with different models to see which one works best for your use case.
License

This project is licensed under the MIT License - see the LICENSE.md file for details.
