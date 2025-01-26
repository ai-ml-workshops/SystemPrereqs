## Demystifying GenAI: Build A ChatGPT App with Vector Store

Welcome!  We will have more than 1 version of the lab exercise: Java being the primary version, with examples also using Python and .Net (Thanks to our Community Contributors!).

### Java
- Preferably using an IDE such as IntelliJ, VS Code, (or any equivalent tooling). CLI is okay too but you may need a bit of experimentation.
- JDK 21.0 or later - Download it from [Adoptium](https://adoptium.net/){:target="_blank"} 
- Maven 3.9.9 or higher (Gradle will be okay too if you prefer it)
_We'll be utilizing Spring AI and the online [spring initializr](https://start.spring.io){:target="_blank"}  to generate the initial project 'frame', so the various library dependencies will be downloaded by default (including Spring Boot, Spring AI, Postgres with PgVector libraries...)
- Conainer Runtimes: [Docker](https://docs.docker.com/get-started/get-docker/){:target="_blank"}  or [Podman](https://podman.io/docs/installation){:target="_blank"} 
- Spring AI reference materials can be found in [here](https://docs.spring.io/spring-ai/reference/)(target="_blank")
- Quarkus Langchain4j reference materials can be found in [here](https://quarkus.io/guides/langchain4j/){:target="_blank"} 

#### Hands-on Repositories

##### Spring AI

![Spring AI](images/spring-ai-integration-diagram-3.png)

- [HelloWorld with OpenAI](https://github.com/ai-ml-workshops/ai-openai-helloworld){:target="_blank"} 
- [HelloWorld with Ollama](https://github.com/ai-ml-workshops/ai-ollama-helloworld){:target="_blank"} 
- [Spring AI with RAG and PgVector (written by Dan Vega)](https://www.danvega.dev/blog/2024/10/22/getting-started-with-spring-ai-rag#building-your-first-rag-application){:target="_blank"} 

##### Quarkus Langchain4j

![Quarkus LangChain4j](images/quarkus-llms-big-picture.png)

- [AI Chatbot](https://github.com/ai-ml-workshops/ai-quarkus-langchain4j-chatbot){:target="_blank"} 
- [Document Retrieval for Language Models with PostgreSQL pgVector store](https://github.com/ai-ml-workshops/ai-quarkus-langchain4j-doc-retrieval){:target="_blank"} 

### OPTIONAL Language Examples:

### Python
- Python 3 (consider installing with python virtual environment like pyenv)
- Python IDE of your choice (Visual Studio Code, PyCharm, etc.)
- Docker or Podman
- OpenAI API key (see instructions below)
- Langchain API key to use LangSmith for debugging (optional). To create account and API key, refer to these [instructions](https://docs.smith.langchain.com/administration/how_to_guides/organization_management/create_account_api_key#create-an-account){:target="_blank"} .
- If you're using Windows, install Git Bash so that you can run the commands below (if using VSCode you can select Git Bash after starting the integrated terminal)

#### Hands-on Repositories

[HelloWorld and The Meal Planner Apps](https://github.com/ai-ml-workshops/meal-planner-chatbot){:target="_blank"} 

### C#

- Visual Studio 2022
- .NET 8
- OpenAI API key (see instructions below)

#### Hands-on Repositories

[OpenAI Hello World example with C#](https://github.com/ai-ml-workshops/openai-csharp-helloworld){:target="_blank"} 
 
### OpenAI API key (needed for any project using any OpenAI model)

- Create an OpenAI free account ([signup for new user](https://platform.openai.com/signup/){:target="_blank"} ).
- **You must add money to your account before generating an Open AI Key.** The minimum amount of $5 should be sufficient. 
  - You can verify your balance on the [billing dashboard](https://platform.openai.com/settings/organization/billing/overview){:target="_blank"} . Make sure you see "Auto recharge is off" below your balance, so that it doesn't automatically charge you when you run out of balance.
- Generate OpenAI key

This [website](https://coding-boot-camp.github.io/full-stack/ai/openai-account-setup-guide){:target="_blank"}  has good step-by-step instructions.

#### HuggingFace (OPTIONAL: only if interested, since we may be showing a few features there)
- HuggingFace Account ([signup for new user](https://huggingface.co/){:target="_blank"} )
- AI-ML-Workshops community organization (OPTIONAL:  Please join our new [AI-ML-Workshops community organization](https://huggingface.co/AI-ML-workshops){:target="_blank"}  for continuous info sharing and learning through the community, beyond the scope of this workshop)

#### Container Runtimes 
If you prefer using a container runtime for the DataStore or Database, instead of local installation.
 - [Docker](https://www.docker.com/){:target="_blank"} 
 - [Podman](https://podman.io/){:target="_blank"} 

#### Database and extension(s) (OPTIONAL: needed if not using Docker image and/or if you prefer manual or local installations)
- PostgreSQL  ([Download site](https://www.postgresql.org/download/){:target="_blank"} )
- [PgVector vector extension](https://github.com/pgvector/pgvector/blob/master/README.md){:target="_blank"} 

***Please check back here for more info, including the Workshop GitHub repo when the lab exercises are ready for you***

### [Presentation Slides](https://bit.ly/42cVqoX){:target="_blank"} 
