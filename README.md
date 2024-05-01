# howto
Command line tool to suggest Linux commands using Azure OpenAI

## Installation
```bash
# Make the file executable, optionally install it in a location accessible by PATH
chmod +x howto
sudo cp howto /usr/local/bin/
# Set up Azure OpenAI parameters (can be placed e.g. in ~/.bash_profile)
export AZURE_OPENAI_API_KEY="your_azure_openai_api_key"
export AZURE_OPENAI_ENDPOINT="https://your_endpoint.openai.azure.com"
export AZURE_OPENAI_MODEL="your_model"
# Usage example
./howto install python on ubuntu
```