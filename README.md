
![Logo](https://miro.medium.com/max/554/1*d-YRTQiEje6nKFfws6aVIQ.png)


# Build Chatbot using ChatGPT and Python




To build a chatbot using ChatGPT and Python, you can connect to ChatGPT via API using your API key. You can install the latest version of the openai package and its dependencies using pip. Once you have installed the openai package, you can import and use the openai module in your Python code. After importing the openai module, you need to set your API key using the openai.api_key property. Here's an example code snippet:

```bash
  import openai

# Set your API key
openai.api_key = 'YOUR_API_KEY'

# Define a function to generate a response
def generate_response(prompt):
    model_engine = 'text-davinci-002' # Or any other GPT model
    response = openai.Completion.create(
        engine=model_engine,
        prompt=prompt,
        max_tokens=100,
        n=1,
        stop=None,
        temperature=0.5,
    )
    return response.choices[0].text.strip()
```
With the generate_response function defined, you can use it to generate responses to prompts. You can also add additional parameters to the Completion.create method to customize the response. For more information on using the openai module to generate responses with ChatGPT.

## Roadmap

- The code starts by importing the openai library.

- Next, it sets up an environment variable called OPENAI_Key with the API key from OpenAI.

- Then it starts a loop that prompts for input and stores it in a variable called prompt.

- The code then checks if the user typed ‘exit’ to stop prompting them for input, which would mean they are done answering questions and want to exit this program.

- If so, keep_prompting is set to False and execution stops running through the loop; otherwise, execution continues until there is no more input left or all 200 tokens have been used up.

- The next line creates a completion object using text-DaVinci-003 as its engine type and prompt as its prompt argument (the string that will be shown when asking users what their question was).

- This completes one task at a time because max_tokens=200 tells us how many tasks can be completed before we need to ask again for new input from our user.

- The code is an example of how to use the OpenAI gym API.

- The code starts by importing the necessary libraries, then opens up a prompt for input from the user and stores it in a variable called prompt.

- The user enters their question which will be stored in response.

- If the user enters exit, then keep_prompting is set to false and if not, then openai completion engine is used to return a list of choices that can be selected from with text associated with each choice.


## 🔗 Links
[![portfolio](https://img.shields.io/badge/my_portfolio-000?style=for-the-badge&logo=ko-fi&logoColor=white)](https://katherineoelsner.com/)
[![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/)
[![twitter](https://img.shields.io/badge/twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white)](https://twitter.com/)

