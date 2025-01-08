# 30 Days DevOps Challenge - Weather Dashboard

Day 1: Building a weather dashboard using AWS S3 and integrating with OpenWeather API

## Project Visualization
For this project, we developed a weather dashboard that fetches real-time weather data for multiple cities through an external API integration (OpenWeather API). This data is automatically stored in AWS S3 Bucket created during the project.

## Features
- Fetches weather data for multiple cities from OpenWeather.
- Stores weather data in an AWS S3 bucket.
- Displays temperature, humidity, and weather conditions.

## Technical Architecture
- **Language:** Python 3.13.1
- **Cloud Provider:** AWS (S3) 
- **External API:** OpenWeather API [Link](https://openweathermap.org/api)
- **Dependencies:** 
  - boto3 (AWS SDK Python used to interact with AWS services like S3)
  - python-dotenv (Manages our environment variables)
  - requests (We are able to make HTTP requests to the OpenWeather API)

## Project Structure
```markdown
weather-dashboard/
  src/
    __init__.py
    weather_dashboard.py
  tests
  .env
  .gitignore
  requirements.txt
```

## Setup Instructions
1. Clone the repository:
   ```bash
   git clone 

2. Navigate to the project directory:
   ```bash
   cd weather-dashboard

3. Install dependencies:
    ```bash
    pip install -r requirements.txt

4. Configure environment variables (.env):
    ```bash
    OPENWEATHER_API_KEY=copy your_api_key
    AWS_BUCKET_NAME=your_unique_bucket_name

5. Configure AWS credentials:
    ```bash
    aws configure
    - AWS Access Key ID
    - AWS Secret Access Key
    - Default region name [eg. us-east-1]
    - Default output format [ eg. json]

6. Run the application:
    ```bash
    python src/weather_dashboard.py

7. View the fetched weather data in your terminal isplaying temperature, humidity, and weather conditions.

8. Navigate to your AWS Console and check your AWS S3 Bucket for weather data files stored in the bucket.

9. Empty your bucket and delete your S3 bucket to avoid incurring any unbudgeted costs.

## Happy Development!
