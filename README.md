# github.io
CornHacks: Your AI Interior Design Assistant for Bathrooms
 
 
Project Overview
 
Welcome to CornHacks, an innovative project inspired by the custom and affordable design philosophy of Studio Banana. Our mission is to make interior design accessible and personalized for everyone, ensuring that every individual feels truly at home in their space. For this hackathon, we focused on bathroom design, developing an AI Interior Design Assistant prototype. Bathrooms, often overlooked by traditional design firms, are integral to our daily lives – we begin and end our days there. We believe everyone deserves a bathroom that feels like a sanctuary.
 
Technology Stack
 
Our project is built as a web application using the following technologies:
Frontend: HTML, CSS, JavaScript
Backend: Custom Python-based RAG (Retrieval Augmented Generation) system, powered by a database of interior design plans, and a chatbot leveraging the Gemini API.
 
How it Works
 
The CornHacks experience is designed to guide users through a personalized bathroom design journey:
Design Questionnaire: The user's journey begins with a brief questionnaire to understand their aesthetic preferences and identify their core design style.
Specific Design Prompt: Following the questionnaire, users are presented with a search prompt box. Here, they can express more specific design requests, such as "minimalistic aesthetic with no cool tones," "industrial style with dark wood," or "bohemian bathroom with lots of plants."
Intelligent Backend (RAG System): This is where our custom database and AI shine.
We developed a database from scratch containing interior design plan images, style types, and detailed text descriptions.
This database is queried using a RAG (Retrieval Augmented Generation) system.
The system computes vector cosine similarity to assess the semantic meaning of phrases in the user's prompt, determining how well the prompt's text matches our database descriptions.
To enhance its understanding of logical relationships, we incorporated regular expressions and declared positive and negative queries. When a prompt is entered, similarity is calculated for both positive and negative aspects. These values are then subtracted (positive - negative) and ranked in descending order to provide the most relevant design matches.
The system is highly flexible and can be modified to integrate with any database (SQL, Salesforce, GCP, AWS).
Personalized Recommendations: The top design matches are returned to the user, providing visual inspiration and detailed descriptions.
Interactive Chatbot: For further customization and support, our site includes a chatbot. Powered by the Gemini API 2.5 (FLASK), this chatbot can:
Discuss important design decisions.
Help with proper budgeting.
Answer any other design-related inquiries.
 
Features
 
Personalized Design Questionnaire: Tailors design suggestions to individual aesthetic preferences.
Semantic Search: Advanced RAG system uses vector cosine similarity for accurate and relevant design retrieval.
Customizable Database Integration: Easily adaptable to various database systems.
Positive/Negative Query Logic: Refined search results by considering desired and undesired elements.
AI-Powered Chatbot: Provides intelligent assistance for design decisions, budgeting, and general inquiries.
User-Friendly Interface: Built with HTML, CSS, and JavaScript for a smooth user experience.
