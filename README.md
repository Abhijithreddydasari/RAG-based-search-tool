# RAG-based-search-tool
## RAG:

Retrieval Augumented Generation is a technique where an LLM incorporates information from external sources (sources that are external to training set) before producing a response.

It mainly takes care of the two drawbacks of LLMs by:
1. Citing the sources of its information (using the external data source)
2. Gives up-to-date information about anything asked 


For obtaining the context related information from the external sources, we can use any method like classification or semantic similarity.

Best definition out there: Retrieval-Augmented Generation (RAG) is a technology that enhances the capabilities of Large Language Models (LLMs) by incorporating retrieval mechanisms to access external knowledge sources during the generation of responses.

![](https://github.com/Abhijithreddydasari/RAG-based-search-tool/blob/main/Project_docs/Working%20of%20RAG.png)


## Working:
![](https://github.com/Abhijithreddydasari/RAG-based-search-tool/blob/main/Project_docs/Workflow.png) <br>

In the image above, the query is fed to the retrieval model which search the knowledge base for relevant docs and then send both the query and docs to the LLM, which then generates the response.

### Advantages:

- Removes the need for retraining data everytime & hence cost-effective implmentation
- LLMs can be fine-tuned to company specific information without customly making changes in it
- Gives up-to-date information when connecting to social media
- Accurate information with source transparancy

## Development of Frontend and Backend:

## **Backend**

### **Technologies Used:**

- **Flask**: Flask is a micro web framework for Python used to develop web applications.
- **SQLite**: SQLite is a lightweight relational database management system used for storing user credentials.
- **Cassandra**: Cassandra is a NoSQL database used for storing trained model embeddings.
- **OpenAI API**: OpenAI API is used for natural language processing tasks, including training and querying the model.
- **PyPDF2**: PyPDF2 is a Python library used for reading PDF files and extracting text from them.
- **Werkzeug**: Werkzeug is a utility library for WSGI (Web Server Gateway Interface) applications in Python.

### **Features:**

- **User Authentication**: Users can register with unique usernames and passwords. Passwords are securely hashed before storing in the database. Authentication is performed securely.
- **Model Training**: Users can upload PDF files, which are processed to extract text. The extracted text is used to train the machine learning model using OpenAI's API. Trained model embeddings are stored in a Cassandra database.
- **Question Answering**: Users can ask questions through a web interface. The system retrieves relevant answers from the trained model stored in the Cassandra database.
- **Web Pages**: The application provides routes for registering, logging in, and accessing protected routes. HTML templates are rendered for user interaction.
- **Security**: The application implements secure password hashing for user authentication. File uploads are restricted to PDF format, and proper validation is performed. A secret key is used for session security.

## **Frontend**

### **Technologies Used:**

- **HTML**: HTML is used for structuring web pages.
- **CSS**: CSS is used for styling the HTML elements and providing visual aesthetics.
- **JavaScript**: JavaScript is used for client-side scripting, enabling dynamic interaction with the web page.
- **Font Awesome**: Font Awesome icons are used for enhanced visual appeal.
- **Google Fonts**: Google Fonts are used to import custom fonts for text elements.

### **Features:**

- **Login Page**: The login page allows users to log in with their registered credentials. It provides a form for entering the username and password.
- **Registration Page**: The registration page allows new users to create an account by providing a username and password.
- **Main Interface**: The main interface provides a chat-like interface for users to ask questions and receive answers from the system. It also allows users to upload PDF files for model training.

## **Usage**

I will soon post a description that properly explains the workflow of the code and how to locally install it and use it for your projects or any other activity.
Till then, watch the following video which explains the project in brief along with execution of the code!
<br>
Video Link: https://drive.google.com/file/d/1CSs2x4dIIl0aYeQLFs_P8MGFwVwI3tMI/view?usp=sharing
<br> <br>
Thank you for reading this far! I hope I made you learn something new today. If you want to suggest any changes or add exciting features, please feel free to submit pull requests.

Thank you!! 😀
