# LLM RAG Demo

## Setup

1. Create a .env file in the project root with the following variables.
    ```bash
    OPENAI_API_KEY=<YOUR_OPENAI_API_KEY>

    NEO4J_URI=<YOUR_NEO4J_URI>
    NEO4J_USERNAME=<YOUR_NEO4J_USERNAME>
    NEO4J_PASSWORD=<YOUR_NEO4J_PASSWORD>
    
    HOSPITALS_CSV_PATH=https://raw.githubusercontent.com/dotslash21/llm-rag-demo/main/data/hospitals.csv
    PAYERS_CSV_PATH=https://raw.githubusercontent.com/dotslash21/llm-rag-demo/main/data/payers.csv
    PHYSICIANS_CSV_PATH=https://raw.githubusercontent.com/dotslash21/llm-rag-demo/main/data/physicians.csv
    PATIENTS_CSV_PATH=https://raw.githubusercontent.com/dotslash21/llm-rag-demo/main/data/patients.csv
    VISITS_CSV_PATH=https://raw.githubusercontent.com/dotslash21/llm-rag-demo/main/data/visits.csv
    REVIEWS_CSV_PATH=https://raw.githubusercontent.com/dotslash21/llm-rag-demo/main/data/reviews.csv
    
    HOSPITAL_AGENT_MODEL=gpt-3.5-turbo-1106
    HOSPITAL_CYPHER_MODEL=gpt-3.5-turbo-1106
    HOSPITAL_QA_MODEL=gpt-3.5-turbo-0125
    
    CHATBOT_URL=http://host.docker.internal:8000/hospital-rag-agent
    ```
2. Run the following command to start the project.
    ```bash
    docker compose up --build
    ```
3. Open the browser and navigate to `http://localhost:3000` to access the application.