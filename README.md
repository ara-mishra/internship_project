# Internship_Project

Customer Support Sentiment Analysis Project

Problem Statement
Build a tool that can analyze customer support voice recordings (from service calls) and extract sentiment and emotion insights. The pipeline:
- Transcribes the voice into text using AssemblyAI
- Processes and classifies the transcript into positive, negative, and neutral sentiments
- Performs emotion classification
- Visualizes the results in an interactive Tableau dashboard

This project includes transcribed/analyzed sample files for three recordings (four customer support calls), along with instructions on how to create your own files for analysis.  

Project Structure 
MP3 audio recordings and their respective transcripts and classifications are uploaded for three recordings. 

Setup Instructions
Python Environment
Required Packages:
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

API_KEY = "your_api_key_here"

Run all cells in the notebook to:
- Upload the .mp3 file
- Transcribe it using AssemblyAI
- Save the transcript to a DataFrame and Excel file

Emotion & Sentiment Classification
1. Copy transcript sentences into a new Excel file
2. Use an AI tool like ChatGPT or Claude
3. Ask:
   “Classify the following lines into emotions such as happy, frustrated, angry, neutral, etc.”
4. Paste the results into Transcript1_Emotion.xlsx accordingly

You can replicate this for other transcripts too.


Tableau Dashboard
Files Needed:
- transcript1_sentiment.xlsx or accordingly 
- Transcript1_Emotion.xlsx or accordingly
- Internship_final.twbx

Steps:
1. Open Tableau Public or Tableau Desktop
2. Load the .twbx file
3. Connect it to your updated Excel files and create a relationship between “text” in both files
4. Review or customize:
- Overall sentiment distribution
- Emotion timeline
- Keywords by sentiment/emotion




