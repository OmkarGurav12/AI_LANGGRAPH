Documentation Workflow Automation

This project is a Python-based workflow automation system that generates business and technical documentation for projects. It uses LangChain to manage agents that produce documents based on a defined workflow graph.

Features:

State Management : Uses a WorkflowState schema to track project data and document paths.

Agents : Modular agents (e.g., BusinessDescriptionAgent, SystemAbstractionAgent) generate specific documents.

Workflow Graph : A StateGraph manages dependencies between agents, ensuring proper execution order.

Document Manager : Automatically saves generated documents in categorized directories.

Customizable : Add new agents or modify the workflow to fit your project needs.

---------
Requirements :-
Python : Python 3.8 or higher.
INSTALL:requirements.txt
ADD your API keys in .env file, or directly in the code
---------




----------------------------------------------------
"ERRORS" :  ValueError: Must provide state_schema or input and output

The error occurs when initializing the DocumentationWorkflow class, specifically in the create_workflow method. The StateGraph object requires a schema (state_schema, input, or output) to be provided, but the code is missing or incorrectly providing this schema.

-----------------------------------------------------
"ERROR2": TypeError: StateGraph.init () got an unexpected keyword argument 'input_type'

The error occurs when initializing the StateGraph object with an unexpected argument (input_type). This indicates that the API for StateGraph does not accept input_type as a valid parameter

----------------------------------------------------

"ERRORS":  TypeError: DocumentationAgent.__init__() missing 2 required positional arguments: 'doc_type' and 'category'

The DocumentationAgent class requires two mandatory arguments (doc_type and category) during initialization, but they are not provided. This results in a TypeError