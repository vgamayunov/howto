# howto
Command line tool to suggest Linux commands using Azure OpenAI

## Installation
Make the file executable, optionally install it in a location accessible by PATH
```bash
chmod +x howto
sudo cp howto /usr/local/bin/
```
Make sure you have `openai` python module installed (`pip install openai`). Optionally, install `azure.identity` module if you plan to use identity to authenticate to Azure OpenAI resource (`pip install azure-identity`).

Set up Azure OpenAI parameters (can be placed e.g. in ~/.bash_profile)
```bash
export AZURE_OPENAI_API_KEY="your_azure_openai_api_key"
export AZURE_OPENAI_ENDPOINT="https://your_endpoint.openai.azure.com"
export AZURE_OPENAI_MODEL="your_model"
```
To use identity instead of API key, set
```bash
export AZURE_OPENAI_USE_IDENTITY=true
```
Usage example
```bash
./howto install python on ubuntu
```
