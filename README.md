
Customer Support Sentiment Analysis Project

Problem Statement:
Build a tool that can analyze customer support voice recordings (from service calls) and extract sentiment and emotion insights. The pipeline:
- Transcribes the voice into text using AssemblyAI
- Processes and classifies the transcript into positive, negative, and neutral sentiments
- Performs emotion classification
- Visualizes the results in an interactive Tableau dashboard

This project includes transcribed/analyzed sample files for three recordings (four customer support calls), along with instructions on how to create your files for analysis.  

Setup Instructions
Python Environment
Required Packages:
- Python 3.10
- assemblyai – for transcribing audio using the AssemblyAI API
- os – standard library for file and path handling
- pandas – for managing and exporting transcript data to Excel
- nltk – for natural language processing
- nltk.sentiment.vader – specifically for sentiment analysis

Install all required libraries using:
pip install assemblyai pandas nltk

AssemblyAI API Setup
- Sign up at https://www.assemblyai.com/
- Get your API key from the dashboard
- In the file, replace the API_KEY placeholder with your key:
- 
How to Run the Code
1. Open the relevant `.ipynb` file for the call recording.
2. Replace the placeholder line with your actual AssemblyAI API key:

   API_KEY = "your_api_key_here"

3. Update the file path to your `.mp3` audio file.
4. Run all notebook cells to:
   - Upload and transcribe the audio
   - Perform sentiment analysis
   - Export results to Excel

Emotion Classification (Manual Step)
1. Open the transcript Excel file.
2. Add a column titled `Emotion`.
3. Use an AI tool (e.g., ChatGPT or Claude) and prompt:

   Classify the following lines into emotions such as happy, rude, polite, neutral, etc.

4. Paste the results into the Excel sheet.
5. Add a `Call ID` column to track which transcript the lines belong to.

Combine sheets of all recordings in a single excel file, Combined_Data

Tableau Dashboard

Steps:
1. Open Tableau Public or Tableau Desktop
2. Load the .twbx file
3. Connect it to your updated Excel file, Combined_Data 
4. Review or customize:
   - Sentiment over time
   - Overall sentiment distribution
   - Emotion breakdown
   - Keyword/emotion insights
   - Filter by `Call ID` to view individual calls













