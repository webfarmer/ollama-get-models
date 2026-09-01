# ollama-get-models

This Python script scrapes information about AI models from the Ollama library website (https://ollama.com/library). It performs the following main tasks:

It first checks if a local HTML file exists. If not, it fetches the webpage content and saves it locally.

It then parses the HTML content using BeautifulSoup to extract details about each model, including name, description, sizes, number of pulls, tags, and last updated date.

The extracted information is printed to the console and also saved as a JSON file.

The script includes error handling for failed web requests and creates necessary directories if they don't exist.

This code allows users to easily obtain and store up-to-date information about available models in the Ollama library without manually browsing the website.

## Usage

```bash
python -m pip install -r requirements.txt
python get_ollama_models.py
```

The script fetches the current library page on every run. If Ollama is temporarily unavailable, it falls back to the last cached HTML response.
