# LangGraph Multi-Agent App

This project demonstrates how to build a multi-agent application using LangGraph. The application leverages LangChain's tools and agents to create a conversational AI system.

## Features

* **Multi-Agent Architecture:** The application employs a multi-agent approach, allowing different agents to handle specific tasks.
* **LangGraph Integration:** LangGraph is used to orchestrate the interactions between agents and manage the application's state.
* **LangChain Tools and Agents:** The application utilizes LangChain's tool and agent framework to perform various actions, such as retrieving information and calling external APIs.
* **Conversational AI:** The application enables users to interact with the system through natural language.


## Installation

1. Install the required libraries:
Use code with caution
bash !pip install --quiet --upgrade langgraph langchain langchain_community langchain-chroma langchain_google_genai wikipedia arxiv

 
2. Set up your API keys:
* Store your Google API Key and LangChain API Key in Colab userdata under the keys `Gemini_Api_Key` and `langchai_api_key` respectively.
* Set the environment variables `GOOGLE_API_KEY`, `LANGCHAIN_TRACING_V2`, `LANGCHAIN_API_KEY`, and `LANGCHAIN_PROJECT` accordingly.

## Usage

1. Run the provided Colab notebook.
2. Initiate a conversation with the agent by providing a natural language query.
3. The agent will utilize its tools and knowledge to respond to your query.

## Example
Use code with caution
input = { "messages": [HumanMessage(content="how to make multi agent app using langraph?")]}

for output in app.stream(input, {"recursion_limit":10}): for key,value in output.items(): print(f"Get response from {key}") print(value) print("----")

## License

This project is licensed under the [MIT License](LICENSE).
