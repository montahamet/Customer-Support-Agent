# Customer-Support-Agent
This project builds an intelligent customer support agent that can understand what users are asking and how they feel. Using LangGraph and Groq’s Llama 3.3 model, the system guides each customer message through a structured workflow, deciding whether it should be handled automatically or passed on to a human agent. The goal is to make early customer interactions faster, more helpful, and more empathetic by responding appropriately to both the intent and emotional tone of each query.

---

### **Key Components**

1. **State Management:** Using TypedDict to define and manage the state of each customer interaction.
2. **Query Categorization:** Classifying customer queries into Technical, Billing, or General categories.
3. **Sentiment Analysis:** Determining the emotional tone of customer queries.
4. **Response Generation:** Creating appropriate responses based on the query category and sentiment.
5. **Escalation Mechanism:** Automatically escalating queries with negative sentiment to human agents.
6. **Workflow Graph:** Utilizing LangGraph to create a flexible and extensible workflow.

---

### **Method Details**

1. **Initialization:** Set up the environment and import necessary libraries.
2. **State Definition:** Create a structure to hold query information, category, sentiment, and response.
3. **Node Functions:** Implement separate functions for categorization, sentiment analysis, and response generation.
4. **Graph Construction:** Use StateGraph to define the workflow, adding nodes and edges to represent the support process.
5. **Conditional Routing:** Implement logic to route queries based on their category and sentiment.
6. **Workflow Compilation:** Compile the graph into an executable application.
7. **Execution:** Process customer queries through the workflow and retrieve results.

---

### **System Workflow**
The following diagram illustrates the complete workflow of the Customer Support Agent, from receiving a customer message to producing a final response or escalation.

<img width="674" height="432" alt="workflow" src="https://github.com/user-attachments/assets/ab118969-f83f-4767-8d2a-30f0e2a08a6f" />


