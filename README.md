# Customer Service Chatbot

An agentic AI customer service chatbot built with LangGraph and Google Gemini.

## What it does
A router reads each customer message and sends it to the right agent:
- **Product agent**: answers laptop feature and pricing questions using a product PDF and price table
- **Orders agent**: looks up order details and updates order quantities
- **Refund agent**: answers questions about the return and refund policy
- **Small talk**: handles greetings and goodbyes

Each agent has a system prompt that defines its role, and conversation memory is kept across turns with LangGraph's MemorySaver.

## How to run
1. Open the notebook in Google Colab.
2. Add your Gemini API key as a Colab Secret named `GOOGLE_API_KEY` (key icon in the sidebar, with notebook access turned on).
3. Run all cells from the top. The notebook downloads the sample data it needs.

## Notes
- API keys are stored in Colab Secrets and are not included in the code.
- Built from the course starter code, with Azure replaced by Gemini and a Refund agent added.
