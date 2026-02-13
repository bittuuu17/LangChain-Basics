
# LangChain with Google Gemini Integration

This notebook demonstrates how to integrate and utilize the Google Gemini Large Language Model (LLM) with the LangChain framework. It covers various aspects of LangChain, from basic model invocation to more advanced features like structured output parsing and LangChain Expression Language (LCEL).

## Table of Contents

1.  **Installation and API Key Setup**: How to install necessary libraries and configure your Google API key.
2.  **Basic Model Invocation**: Making a simple call to the Gemini model.
3.  **Prompt Templates**: Using `PromptTemplate` for single-turn interactions with dynamic inputs.
4.  **Chat Prompt Templates**: Using `ChatPromptTemplate` for multi-turn conversations, including system and human messages.
5.  **LangChain Expression Language (LCEL)**: Building powerful and flexible chains of components.
    *   Simple chains (`prompt | llm | output_parser`)
    *   Multi-step chains (`topic_chain | story_chain`)
6.  **Structured Output Parsing**: Extracting structured data (e.g., JSON) from LLM responses using Pydantic models and `JsonOutputParser`.

## Getting Started

To run this notebook, you will need:

*   A Google API Key (configured as a Colab secret named `GOOGLE_API_KEY`).
*   The `langchain` and `langchain-google-genai` libraries installed.

Follow the cells sequentially to understand each concept.

## Key Concepts Demonstrated

*   **`ChatGoogleGenerativeAI`**: The LangChain wrapper for the Gemini model.
*   **`llm.invoke()`**: The primary method for sending prompts to the LLM.
*   **`PromptTemplate`**: Structuring single-turn prompts.
*   **`ChatPromptTemplate`**: Structuring multi-turn chat prompts.
*   **`StrOutputParser`**: Simple parser to get string output from LLM responses.
*   **`JsonOutputParser` and `Pydantic`**: Defining and parsing structured data from LLM outputs.
*   **`LCEL` (LangChain Expression Language)**: The pipe operator (`|`) for creating sequential chains.
*   **`RunnablePassthrough`**: For managing input to complex chains.

This notebook provides a foundational understanding of building LLM-powered applications using LangChain and Google Gemini.
