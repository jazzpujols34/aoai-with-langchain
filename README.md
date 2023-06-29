# Azure OpenAI Language Model

This project demonstrates how to use Azure OpenAI's language model for various tasks such as generating responses to prompts, running a conversation chain, and more.

## Installation

Clone the repository and install the necessary packages:

```
git clone https://github.com/yourusername/your-repo-name.git
cd your-repo-name
pip install -r requirements.txt

---
## Usage

The main script demonstrates various tasks:

1. Setting up OpenAI API configurations.

2. Initializing AzureOpenAI with deployment and model names.

3. Running the language model to get responses to prompts.

4. Defining a prompt template for product naming.

5. Running the language model with a formatted prompt.

6. Initializing and running a language model chain with input variables.

7. Initializing memory for a conversation.

8. Initializing and running a conversation chain with the language model.

9. Running an interactive conversation loop.

## Environment Variables

To run this project, you will need to add the following environment variables to your .env file:

`OPENAI_API_TYPE`
`OPENAI_API_KEY`
`OPENAI_API_BASE`
`OPENAI_API_VERSION`

## Examples

```
# Initialize AzureOpenAI with deployment and model names
llm = AzureOpenAI(deployment_name="davinci", model_name="text-davinci-003")

# Example: Run the LLM to get the capital of Italy
print(llm("What is the capital of Italy?"))

# Initialize LLMChain with the LLM and prompt
chain = LLMChain(llm=llm, prompt=prompt)

# Example: Run the chain with input variables
print(chain.run(product_type="pair of sunglasses", benefit='high altitude protection'))
```

## Contributing

Contributions are always welcome! 