# Budget Summarizer Web Application

## Overview
The Budget Summarizer is a web application designed to process and summarize the Indian Union Budget speech for a specific financial year. It uses NLP techniques to categorize content sector-wise, extract numerical data, and present an easy-to-understand summary for users.

---

## Features

### 1. Input Handling
- Accepts a financial year (e.g., 2023-2024) as user input.

### 2. Speech Processing
- Retrieves the Union Budget speech for the selected year.
- Processes the speech using Natural Language Processing (NLP) to break it into sections based on economic sectors.

### 3. Data Extraction
- Extracts numerical data such as allocations, expenditures, and key statistics for each sector.

### 4. Summarization
- Generates a concise, sector-wise summary highlighting the major points and numerical data from the speech.

### 5. Output Presentation
- Displays the summary in an organized, user-friendly format with sector-wise breakdowns.

---

## Technology Stack

### Frontend:
- **React.js**: For building an interactive and dynamic user interface.

### Backend:
- **Flask**: For server-side logic and API development.
- **Python**: For Natural Language Processing and data handling.

### Additional Tools:
- **NLP Libraries**: Such as NLTK or spaCy for speech processing and summarization.
- **Data Visualization**: Libraries like Chart.js or D3.js (optional for graphical representation).

---

## Installation and Setup

### Prerequisites
- **Python** (v3.8 or higher)
- **Node.js** (v14 or higher)
- **pip** (Python package installer)
- **Git**

### Steps

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/budget-summarizer.git
   cd budget-summarizer
   ```

2. **Backend Setup**:
   ```bash
   cd backend
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   pip install -r requirements.txt
   python app.py
   ```
   The backend will run on `http://127.0.0.1:5000`.

3. **Frontend Setup**:
   ```bash
   cd frontend
   npm install
   npm start
   ```
   The frontend will run on `http://localhost:3000`.

---

## Usage

1. Navigate to the **Landing Page**.
2. Select a financial year from the dropdown list.
3. View the sector-wise summary and numerical data extracted from the budget speech.

---

## API Endpoints

### 1. **GET /api/speech/{year}**
- Retrieves the budget speech for the specified financial year.

### 2. **POST /api/summarize**
- Processes and summarizes the speech.
- Input: Financial year.
- Output: JSON with sector-wise breakdown and numerical data.

---

## Test Cases

### Test Case 1: User Input Handling
- **Input**: User selects `2023-2024` from the dropdown.
- **Expected Output**: The system retrieves and processes the speech for the selected year.

### Test Case 2: Speech Summarization
- **Input**: Speech data for a financial year.
- **Expected Output**: A JSON response with sector-wise summaries and numerical data.

---

## Future Enhancements
- Integration with live speech transcription services.
- Advanced visualizations for data insights.
- Multilingual support for speech processing and summaries.

---

## References
- [Official Union Budget Speeches](https://www.indiabudget.gov.in/bspeech.php)
- NLP Libraries Documentation: [spaCy](https://spacy.io/), [NLTK](https://www.nltk.org/)

---

## License
This project is licensed under the MIT License. See the LICENSE file for details.
