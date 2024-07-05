# Application Tracking System(ATS)
 An intelligent Application Tracking System that evaluates resumes based on job descriptions using Google's Generative AI.
 <p align="center">
     <img width="500" alt="ats-1" src="https://github.com/Sreepriya06/Application-Tracking-System/assets/108683400/a1b515d2-6bb4-42cd-9c15-770dac002a4d">
<img width="500" alt="ats-2" src="https://github.com/Sreepriya06/Application-Tracking-System/assets/108683400/a6551b14-1205-46e0-925a-8342d57ec626">
<img width="500" alt="ats-3" src="https://github.com/Sreepriya06/Application-Tracking-System/assets/108683400/e6218756-5901-4942-97fd-7196e83843f4">
 </p>



## Features

- PDF resume parsing
- Job description matching using Google's Gemini-Pro AI model
- Visual representation of match percentage
- Chat history storage and retrieval
- Responsive Streamlit web interface

## Prerequisites

- Python 3.7+
- Streamlit
- PyPDF2
- python-dotenv
- google-generativeai

## Setup

1. Clone the repository:
   ```
   git clone https://github.com/your-username/Application-Tracking-System.git
   cd Application-Tracking-System
   ```


2. Install the required packages:
   ```
   pip install -r requirements.txt
   ```
4. Create a `.env` file in the project root and add your Google API key:
   ```
   GOOGLE_API_KEY=your_api_key_here
   ```
5. Run the Streamlit app:
   ```
   streamlit run app.py
   ```
## Usage

1. Enter the company name and job role.
2. Paste the job description in the text area.
3. Upload your resume in PDF format.
4. Click "Submit" to get an analysis of your resume.

## Features Explained

### Resume Parsing
PyPDF2 is used to extract text from uploaded PDF resumes.

### AI-Powered Analysis
Google's Generative AI (Gemini-Pro model) analyzes the resume against the job description, providing:
- JD Match percentage
- Missing keywords
- Profile summary

### Visual Feedback
A circular progress indicator visually represents the JD Match percentage.

### Chat History
Previous analyses are stored and can be accessed from the sidebar.

## File Structure

- `app.py`: Main application file
- `requirements.txt`: List of Python dependencies
- `.env`: Environment variables (not in repository)
- `chat_history.json`: Stores chat history (generated on first run)

