# Demystifying Generative AI

**Welcome!** This tutorial guides you through creating a generative AI application – **a ChatGPT-like model** – with the power of Vector Stores. **We'll start with Java**, providing a hands-on experience. Afterward, you can explore equivalent implementations in *Python and C#*.

**Review and deepen your understanding with the [Presentation Slides](https://bit.ly/4pubCtH)**.

##All exercises are conducted using Oracle LiveLab’s cloud-based sandboxes.

##All you need is your laptop and an **Oracle Account**. 

1) The account is free and can be created here:

[https://profile.oracle.com/myprofile/account/create-account.jspx](https://profile.oracle.com/myprofile/account/create-account.jspx)
 
**If you do not have the account, please create it now, otherwise you can skip this step**.  

2) Reserve an Oracle LiveLab Sandbox (free-tier) **HIGHLY SUGGESTED: Advanced Reservation**

[https://bit.ly/3NdQhHN](https://bit.ly/3NdQhHN)

3) Press the ***Start*** button on the upper right corner

4) Press "**Run on LiveLabs Sandbox**"

5) Sign into your Oracle Account (_if you have not signed in yet_)

6) - Verify your email address
   - Select the time zone (US-Eastern)
   - IF YOU ARE DOING THIS STEP IN ADVANCE (before the workshop):
      - Deselect "Start Workshop Now?"
      - Enter the Workshop Date for "Choose a date to attend":  **13-Jan-2026**
      - Enter the Workshop Time for "Choose a time to attend":  **13:00 / 1:00PM**
   - OR, IF YOU ARE DOING THIS STEP DURING THE WORKSHOP:
      - Select "Start Workshop Now?"
   


# OPTIONAL SECTION 

**IF you are interested in trying the Java / Quarkus, Python, and/or C# samples, you are welcome to continue working through this particular section of the guideline**.

## 1. Environment Setup

### 1.1. OpenAI API key

- [Create an OpenAI free account](https://platform.openai.com/signup/)
  - **You need to fund your account before generating an Open AI Key.** The minimum amount of **$5** should be sufficient. 
  - Verify your balance on the [billing dashboard](https://platform.openai.com/settings/organization/billing/overview). 
  - Make sure you see **Auto recharge is off** below your balance, so that it doesn't automatically charge you when you run out of balance.
- Generate OpenAI key.

Fine more information on the [OpenAI Account Setup Guide](https://coding-boot-camp.github.io/full-stack/ai/openai-account-setup-guide).

If you are interested in dealing with LLMs from HuggingFace, follow the instructions below:
- [Sign up for a new account in HuggingFace](https://huggingface.co/)
- [AI-ML-Workshops community organization](https://huggingface.co/AI-ML-workshops)
  - Feel free to join the new AI-ML-Workshops community organization for continuous information sharing and learning through the community, beyond the scope of this workshop

### 1.2. Container Runtimes 

Install Docker or Podman to run the DataStore or Database. In the **Quarkus** exercises, [Quarkus Dev Service for PostgreSQL](https://quarkus.io/guides/databases-dev-services) will be used to start the PostgreSQL container **automatically** based on your container runtime environment.

 - [Docker](https://www.docker.com/)
 - [Podman](https://podman.io/)

If you prefer to install the PostgreSQL database and pgVector extension locally, follow the instructions below:

- [PostgreSQL installation locally](https://www.postgresql.org/download/)
- [PgVector vector extension](https://github.com/pgvector/pgvector/blob/master/README.md)

## 2. Java Excerises

### 2.1. Prerequisites

- Preferably using an IDE such as IntelliJ, VS Code, (or any equivalent tooling). CLI is okay too but you may need a bit of experimentation.
- JDK 25.0 - Download it from [Adoptium](https://adoptium.net/temurin/releases/?version=25)
- Maven 3.9.9 or higher (Gradle will be okay too if you prefer it)
_We'll be utilizing Spring AI and the online [spring initializr](https://start.spring.io) to generate the initial project 'frame', so the various library dependencies will be downloaded by default (including Spring Boot, Spring AI, Postgres with PgVector libraries)
- Conainer Runtimes: [Docker](https://docs.docker.com/get-started/get-docker/) or [Podman](https://podman.io/docs/installation)
- Spring AI reference materials can be found in [here](https://docs.spring.io/spring-ai/reference/)
