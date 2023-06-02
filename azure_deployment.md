# Flask App Apis to Scrape
APIs to Scrape Flask App

## Before deploying
- First of all, make sure you have created a proper requirements.txt containing the following:

Flask>=2.2
Flask-SQLAlchemy>=3.0.2
SQLAlchemy>=1.4.25
Gunicorn==20.1

- Next, make sure that the application file is called app.py (not main.py or anything else, this disrupts the App)

## Deploying the Flask App

- Install Azure CLI
- Go to the specific directory in the terminal
- Run 'az login' and log in using your credentials
- Run the following command to create the webapp :

az webapp up --sku F1 --name <app-name> --resource-group <resource-group-name>

replace <app-name> with your app name and <resource-group-name> with the name of your desired resourcegroup)

- You can replace F1 with your preferred price tier.
- If you make changes to the Flask App, you can redeploy using the command 'az webapp up'


