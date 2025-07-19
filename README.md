
## ✅ Challenge 1B - Multi-Collection PDF Persona Summarizer

### 📄 Problem Statement

For each collection of PDFs and questions, generate answers per persona and output them in a structured format.

### 🗂️ Folder Structure

Challenge_1b/
├── Collection 1/
│   ├── PDFs/
│   ├── challenge1b_input.json
│   └── challenge1b_output.json
├── Collection 2/
├── Collection 3/
├── process_collections.py
├── requirements.txt
└── README.md


### ⚙️ Setup Instructions

1. **Navigate to Challenge 1B:**

   cd adobe-hackathon/Challenge_1b


2. **Install Dependencies:**

   pip install -r requirements.txt
   
3. **Run the Script:**

   python process_collections.py
   
### 📥 Input Format (`challenge1b_input.json`)

{
  "persona": "Manager",
  "questions": [
    "What is the leave policy?",
    "Who to contact for reimbursements?"
  ]
}


### 📤 Output Format (`challenge1b_output.json`)

{
  "persona": "Manager",
  "answers": [
    "The leave policy allows 30 days per year...",
    "Contact HR or finance@example.com..."
  ]
}

### 🧠 Approach

* Parse PDFs using **PyMuPDF**
* Search for relevant content by matching questions to document spans
* Extract context-aware answers using heuristics or basic NLP


### 🛠 Requirements

PyMuPDF==1.22.5