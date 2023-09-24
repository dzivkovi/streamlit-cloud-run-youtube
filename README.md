# Uber Pickups in NYC Streamlit App

This app visualizes Uber pickups in NYC. It's built using Streamlit and can be deployed locally, on Streamlit's Community Cloud, or on Google Cloud Run.

## 1. Local Deployment

To run this app locally, follow these steps:

1. Clone the repository to your local machine.
2. Navigate to the project directory.
3. Install the required Python packages.
4. Run the Streamlit app.

```bash
git clone <repository_url>
cd <project_directory>
pip install -r requirements.txt
streamlit run app.py
```

## 2. Streamlit Community Cloud Deployment

You can also deploy this app on Streamlit's Community Cloud. Here's how:

1. Fork the repository on GitHub.
2. Sign in to [Streamlit Cloud](https://share.streamlit.io/).
3. Click on 'New App' and select the GitHub repository you just forked.
4. Choose the branch and enter the path to your Streamlit app script.
5. Click 'Deploy' to deploy the app.

You can view the deployed app here: [https://uber-pickups-in-nyc.streamlit.app/](https://uber-pickups-in-nyc.streamlit.app/).

## 3. Build and deploy on Google Cloud Run

1. Command to build the application. PLease remeber to change the project name and application name
2. Command to deploy the application

``` bash
gcloud builds submit --tag gcr.io/<ProjectName>/<AppName>  --project=<ProjectName>
gcloud run deploy --image gcr.io/<ProjectName>/<AppName> --platform managed  --project=<ProjectName> --allow-unauthenticated
```
