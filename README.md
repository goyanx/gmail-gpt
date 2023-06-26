# Gmail-GPT

Gmail-GPT is a tool that uses OpenAI's GPT-4 model to analyze and categorize emails, providing a structured output that can be used for business automation. It extracts key information from the email content, such as the company name, product details, and the amount of product, and categorizes the email based on its content. It also provides a priority score for the email based on its potential business opportunity.

## Features

- Extracts key information from emails.
- Categorizes emails into different categories like sales, customer support, consulting, partnership, etc.
- Provides a priority score for each email based on its potential business opportunity.
- Suggests the next step to move the conversation forward.
- Converts unstructured email data into structured JSON format.

## How it Works

The tool uses OpenAI's GPT-4 model with the function calling feature to analyze the content of the email. It extracts key information such as the company name, product details, and the amount of product. It also categorizes the email based on its content and provides a priority score for the email based on its potential business opportunity. The tool then suggests the next step to move the conversation forward.

The tool is implemented as an API endpoint using FastAPI. When a new email is received, a POST request is sent to the API with the email content. The API then processes the email and returns a structured JSON response with the extracted information.

## Setup

1. Clone the repository.
2. Install the required libraries listed in the `requirements.txt` file.
3. Set up your OpenAI API key in a `.env` file.
4. Run the server using the command `uvicorn main:app --host 0.0.0.0 --port 10000`.

## Usage

Send a POST request to the API endpoint with the email content in the request body. The API will return a structured JSON response with the extracted information.

## Deployment

The tool can be deployed to a cloud service like Render. Once deployed, the API can be called whenever a new email is received to automatically analyze and categorize the email.

## Integration

The tool can be integrated with other services like Gmail and Google Sheets using a platform like Zapier. For example, a workflow can be set up to trigger the tool whenever a new email is received in Gmail. The tool then analyzes the email and the output is automatically added to a Google Sheet.

## Disclaimer

This tool is an experiment and is not intended for production use. The accuracy and reliability of the tool's output depend on the performance of the underlying GPT-4 model.

## License

This project is licensed under the terms of the MIT license.

## Contact

For any queries or suggestions, please open an issue on GitHub.

## Acknowledgements

This project was inspired by the capabilities of OpenAI's GPT-4 model and its potential for business automation. The project also leverages the FastAPI library for creating the API endpoint and Render for deployment.

## Video Tutorial

For a detailed walkthrough of the project, check out this [YouTube video](https://www.youtube.com/watch?v=AetT0ZqwNqY).
