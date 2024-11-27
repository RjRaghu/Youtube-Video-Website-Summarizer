# Youtube-Video-Website-Summarizer
LangChain: Summarize Text From YouTube or Website
Overview
This Streamlit app leverages LangChain and the ChatGroq model to provide an AI-powered summary of text content from YouTube videos and websites. You can input a URL, and the app will extract and summarize the content using a custom prompt template.

Features
Summarize YouTube Video Transcripts: Fetches the transcript of a YouTube video and provides a concise summary.
Summarize Website Content: Extracts and summarizes the main text content from a given website.
Groq API Integration: Uses the Groq API with the ChatGroq model to process and summarize content effectively.
Installation and Setup
Clone the repository:

bash
Copy code
git clone <https://github.com/RjRaghu/Youtube-Video-Website-Summarizer/commits/eff01b3b7b89fa527be0552c2791f50c843ae2f0/>
cd <your-project-directory>
Install dependencies: Make sure you have Python 3.8+ installed, then use the following command to install required libraries:

bash
Copy code
pip install -r requirements.txt
Ensure that requirements.txt includes:

plaintext
Copy code
streamlit
requests
bs4
validators
langchain
langchain-groq
youtube-transcript-api
Run the app:

bash
Copy code
streamlit run app.py
Replace app.py with the filename of your Python script if different.

Usage
Start the app by running streamlit run app.py.
Enter your Groq API Key in the sidebar. This key is required for the ChatGroq model.
Input the URL of the YouTube video or website you wish to summarize.
Click the "Summarize the Content from YT or Website" button.
The app will process the content, summarize it, and display the summary.
Code Explanation
Libraries Used
Streamlit: Used for building the web interface.
Requests and BeautifulSoup: Used for web scraping to extract content from websites.
LangChain and ChatGroq: For building and running the language model to summarize the content.
YouTube Transcript API: Extracts transcripts from YouTube videos.
Key Functions
fetch_website_content(url): Fetches and extracts text from a website.
run() method of the LangChain chain: Processes the input document and returns a summary.
Example Workflow
Open the app in your browser.
Provide the Groq API Key and input a valid YouTube or website URL.
Click "Summarize the Content from YT or Website" to receive the summarized text.
Troubleshooting
Invalid API Key: Ensure that the Groq API Key is correct and active.
URL Issues: The app supports URLs with the youtube.com, youtu.be, and general website links.
Transcript Availability: Not all YouTube videos have transcripts, especially if they are in certain languages or have no captions enabled.
Contributing
Feel free to fork this project, make improvements, and submit pull requests. For any issues or feature requests, please open an issue on GitHub.

License
This project is licensed under the MIT License. See the LICENSE file for more details.

Acknowledgements
LangChain and ChatGroq for powerful language model capabilities.
YouTube Transcript API for extracting video transcripts.
