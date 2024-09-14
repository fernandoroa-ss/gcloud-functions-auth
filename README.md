## Google Cloud functions - Authenticated

### Starting a project

To start a new project in Google Cloud, go one of this links
[firebase console](https://console.firebase.google.com)  
[projects console](https://console.cloud.google.com/cloud-resource-manager)

### Billing Account

At some point, gcloud will ask to associate the project to a billing account
[billing account](https://console.cloud.google.com/billing)

### Requirements

Install gcloud CLI  
[gcloud CLI](https://cloud.google.com/sdk/docs/install#deb)

### Workflow

```
# Log in
gcloud auth login --no-launch-browser

# Check active account
gcloud auth list

# Check project names and IDs
gcloud projects list

# activate project
gcloud config set project [project-id]
```

### Deploying apps

#### Check List

- `main.py` file

```
gcloud functions deploy hello_world --runtime=python312 --trigger-http --source=.
```
