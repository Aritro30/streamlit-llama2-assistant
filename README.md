
# Llama 2 Chatbot Streamlit App

## Overview

This Streamlit app, titled "Llama 2 Chatbot," integrates the LLaMA2 chatbot model from Replicate and a sentiment analysis model to create a chat interface where users can interact with the chatbot.

## Dependencies

- [Streamlit](https://streamlit.io/)
- [Transformers](https://huggingface.co/transformers)
- [Replicate](https://replicate.ai/)

## Setup

1. **Install required libraries:**
   ```bash
   pip install streamlit transformers replicate
Set up Replicate credentials:

    Obtain an API token from Replicate.
    Store the token in your Streamlit secrets under the name 'REPLICATE_API_TOKEN'.

Run the Streamlit app:


    streamlit run your_app.py

## App Components
1. **Title and Replicate Credentials:**

    The app's title is set using st.set_page_config.
    Replicate API token is obtained from the user through a password input in the Streamlit sidebar.

2. **Model Selection and Parameters**

    Users can choose between two LLaMA2 models: 'Llama2-7B' and 'Llama2-13B'.
    Parameters such as temperature, top_p, and max_length can be adjusted using sliders.
    A link to a blog post on building the app is provided.

3. **Chat Interface**

    The chat interface displays the conversation history between the user and the assistant.
    Users can input messages, and the assistant's responses are generated using the LLaMA2 model.
    Sentiment analysis results for the user's input are displayed in the sidebar.

4. **Clear Chat History**

    A button in the sidebar allows users to clear the chat history.

## Usage

    Enter your Replicate API token in the sidebar.
    Choose a LLaMA2 model and set parameters.
    Input messages in the chat interface.
    The assistant responds using the LLaMA2 model.
    Optionally, clear the chat history using the provided button.

Note: The LLaMA2 models are hosted on Replicate, and their tokens are embedded in the code.
    Streamlit Documentation
    Transformers Documentation
    Replicate Documentation
