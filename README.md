# SQL-based-text-to-JSON-conversion-using-LLM

## Introduction:
Companies and marketing firms face challenges managing vast data. To address this, they convert SQL text queries to JSON for efficient storage, offering compactness, flexibility, and streamlined integration for scalable data management.

## About:
In this project, we've harnessed Falcon7B, a powerful open-source LLM model equipped with 7 billion parameters. This Falcon model, is used for various Natural Language Processing tasks, operates seamlessly through the utilization of transformers and PyTorch, enabling robust and versatile language processing capabilities. The user inputs text in SQL format (e.g., "number of users"), and our model swiftly transforms this text into a JSON format. To enhance its performance, we employ libraries like peft and lora, optimizing the model to achieve superior results in this conversion process. The Falcon model used in this project is `vilsonrodrigues/falcon-7b-instruct-sharded` from Hugging Face.

## Schema:
### The 'users' table schema:
(id, name, email, phone_number, country, gender, timezone, avatar, is_active, access_token, refresh_token, create_date, meeting_id, is_zoom, zoom_link, meeting_preference, user_role, is_onboarded, zoom_refresh_token, city, work_place, about, language, zip, zoom_user_id, permanent_meeting_location, wake_time, primary_calendar_id, provider_id, zoom_user_email, primary_conference_id)

### The 'meetings' table schema:
(id, host_id, title, description, location, link, start_datetime, end_datetime, request_id, meeting_generated, created_date, type, event_id, nlp_output, calendar_id, account_user_id)

## Requirement Specification:
### Software Requirements:
- Python Version: We are utilizing Python version 3.10 (64-bit)
- Pip installs: !pip install -q trl transformers accelerate peft datasets bitsandbytes einops tiktoken
