**n8n Query Bot Documentation**

**Overview**

This workflow enables natural-language querying of a PostgreSQL database using a Google Gemini-powered AI Agent inside n8n. It accepts a user’s question through a webhook, interprets the request using a Gemini model, retrieves the required database metadata, runs SQL queries, and responds with natural-language answers. It also includes a simple memory component that helps with smooth handling of follow-up questions in a conversation like manner with the user. It is especially useful for non-technical questions and being able to query an SQL Database without prior knowledge about SQL queries.


**Use Cases**

●	Answering questions like:

	• “How many tickets did we sell?”
	• “Which drink earned the most?”
	• “Compare venue and event revenue.”
      _Based on the provided DB_
      
●	Also capable of answering further questions on things like how the answer was given including provided the executed SQL query.

●	This is also transferrable among any and all databases and so is easily replicable and can be applied to most if not all SQL databases.

**These are the tools used to build the query bot : **

**1.	n8n : **
```●	Open source workflow automation tool. 
●	It uses docker to run locally on Port : 5678
●	The building platform UI can be found at: http://localhost:5678/```

**2.	Postgres : **
<code>```●	Used keep the Database up and running
●	It uses docker to run locally on Port : 5432```</code> 

**3.	Google Gemini : **
<code>```●	Used as the main LLM (Can be swapped to other models as well)
●	An API key using AI studio currently running on their free tier
●	Recommended gemini model : models/gemini-2.5-pro
●	Other workable models : models/gemini-2.5-flash , models/gemini-2.0-pro-exp , models/gemini-2.0-flash , models/gemini-1.5-pro-latest ,  models/gemini-1.5-pro. (All of these have varying degrees of success)```</code> 

**4.	Memory Buffer : **
<code>```●	Currently using a local n8n simple memory storage tool for ease of use. 
●	Other compatible tools include : MongoDB Chat memory , Motorhead , Postgres Chat memory , Redis chat memory , Xta , Ze ```</code> 

