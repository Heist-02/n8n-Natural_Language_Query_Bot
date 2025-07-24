n8n Query Bot Documentation

Overview
This workflow enables natural-language querying of a PostgreSQL database using a Google Gemini-powered AI Agent inside n8n. It accepts a user’s question through a webhook, interprets the request using a Gemini model, retrieves the required database metadata, runs SQL queries, and responds with natural-language answers. It also includes a simple memory component that helps with smooth handling of follow-up questions in a conversation like manner with the user. It is especially useful for non-technical questions and being able to query an SQL Database without prior knowledge about SQL queries.


Use Cases
●	Answering questions like:

	• “How many tickets did we sell?”
	• “Which drink earned the most?”
	• “Compare venue and event revenue.”
      _Based on the provided DB_
      
●	Also capable of answering further questions on things like how the answer was given including provided the executed SQL query.
●	This is also transferrable among any 
