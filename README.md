# Langchain Notebooks

A collection of notebooks from my own experimentation with Langchain.

## Environment Setup

OpenAI:

```bash
export OPENAI_API_KEY=<your OpenAI API key>
```

Azure OpenAI:
```bash
# Set this to `azure`
export OPENAI_API_TYPE=azure
# The API version you want to use: set this to `2022-12-01` for the released version.
export OPENAI_API_VERSION=2022-12-01
# The base URL for your Azure OpenAI resource.  You can find this in the Azure portal under your Azure OpenAI resource.
export OPENAI_API_BASE=https://your-resource-name.openai.azure.com
# The API key for your Azure OpenAI resource.  You can find this in the Azure portal under your Azure OpenAI resource.
export OPENAI_API_KEY=<your Azure OpenAI API key>
```

```python
# Import Azure OpenAI
from langchain.llms import AzureOpenAI
# Create an instance of Azure OpenAI
# Replace the deployment name with your own
llm = AzureOpenAI(deployment_name="text-davinci-002-prod", model_name="text-davinci-002")
# Run the LLM
llm("Tell me a joke")
```