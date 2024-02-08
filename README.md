## Interview GPT App

This Flask application serves as an interface for generating interview questions based on job descriptions and skills provided.

### Setup Instructions

1. Clone the repository.
2. Install the required dependencies using `pip install -r requirements.txt`.
3. Set up a `.env` file with the required environment variables:

OPENAI_API_KEY=<your_openai_api_key>


4. Run the Flask application using `python app.py`.

### Endpoints

- **/fetch_skills** (POST):
- **Input**: JSON object containing `job_description` and `name`.
- **Output**: Extracts soft skills, technical skills, and estimated years of experience from the job description. Returns retrieved skills.

- **/generate_soft_skill_questions** (POST):
- **Input**: JSON object containing `soft_skills`, `name`, and `experience`.
- **Output**: Generates soft skill related questions based on the provided soft skills and experience.

- **/generate_technical_questions** (POST):
- **Input**: JSON object containing `technical_skills`, `name`, and `experience`.
- **Output**: Generates technical skill related questions based on the provided technical skills and experience.

### How to Use

1. Send a POST request to the appropriate endpoint with the required input data.
2. Retrieve the generated questions and other relevant information from the response.

### Important Notes
1. Ensure that the OpenAI API key is correctly set in the .env file.
2. Adjust the URL in the example usage to match your deployment environment.

