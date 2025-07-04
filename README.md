🧾 Legal Document Classification Tool
Automatically classify legal documents such as NDAs, Contracts, Service Agreements, MOUs, and more using IBM watsonx.ai foundation models with prompt-based AI.

🚀 Features
🔍 Classifies legal document summaries into types (NDA, Contract, Lease, etc.)

🤖 Uses IBM watsonx.ai's granite-13b-instruct-v2 model with few-shot prompting

📄 Uploads CSV with document summaries

🧠 Predicts type using foundation model

📥 Exports results to a new CSV file

🧠 How It Works
Upload a legal_docs.csv file with legal document summaries

Prompt Engineering with a few examples guides the model

The AI model predicts the document type

Predictions are saved in classified_legal_docs.csv

📁 File Structure
pgsql
Copy
Edit
├── legal_docs.csv                 # Input file with document summaries
├── Legal_Classification.ipynb    # Main Colab notebook
└── classified_legal_docs.csv     # Output file with predicted types (generated by code)
🛠️ Technologies Used
IBM watsonx.ai

ibm-watson-machine-learning Python SDK

Google Colab

Python, pandas, numpy

Prompt Engineering (few-shot classification)

📥 How to Use
Clone this repo or open the notebook in Google Colab

Upload your legal_docs.csv file

Run all cells

Download the output classified_legal_docs.csv

📌 Sample legal_docs.csv Format
c
Copy
Edit
document_id,summary
1,"This agreement ensures confidentiality between two parties."
2,"This contract outlines payment terms for services."
✅ Output Example
c
Copy
Edit
document_id,summary,predicted_type
1,"This agreement ensures confidentiality between two parties.",NDA
2,"This contract outlines payment terms for services.",Contract
