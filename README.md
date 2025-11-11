Cold Mail Generator
Cold email generator for services company using groq, langchain and streamlit. It allows users to input the URL of a company's careers page. The tool then extracts job listings from that page and generates personalized cold emails. These emails include relevant portfolio links sourced from a vector database, based on the specific job descriptions.

Imagine a scenario:

Nike needs a Principal Software Engineer and is spending time and resources in the hiring process, on boarding, training etc
Atliq is Software Development company can provide a dedicated software development engineer to Nike. So, the business development executive (Mohan) from Atliq is going to reach out to Nike via a cold email.


Architecture Diagram


Set-up
To get started we first need to get an API_KEY from here: https://console.groq.com/keys. Inside app/.env update the value of GROQ_API_KEY with the API_KEY you created.

To get started, first install the dependencies using:
langchain==0.2.14
langchain-community==0.2.12
langchain-groq===0.1.9
unstructured==0.14.6
selenium==4.21.0
chromadb==0.5.0
streamlit==1.35.0
pandas==2.0.2
python-dotenv==1.0.0
Run the streamlit app:

streamlit run app/main.py
