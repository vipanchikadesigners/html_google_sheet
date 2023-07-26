# Transfer  HTML form data to Google Sheets without third party softwares

A lot of my clients asked me  that there is any option to collect html form data to google sheet directly without any kind of thirdparty softwares.

yes there is an option to collect and transfer html data to google sheet without any kind of thirdparty softwares.For this follow the below steps and this will help you to complete the task.

### 1. The first step is create a google sheet file for collecting data

1. Go to [Google Sheets](https://sheets.google.com) and create a new sheet. This is where we'll store the html form data.

2. Set the following headers in the first row:

you must enter the same name which you use in the html code as your google form title.

### 2. The second step is create a Google App Script

Click on `Extensions -> Apps Script`. This will open new Google Script. Rename it to something like _"mail_list"_.

Replace the `myFunction() { ...` section with the following code snippet which is added in this project and then save the project
### 3. Run the initialSetup function

Then press the run button .If you click on the run button then You should see a modal asking for permissions. Click `Review permissions` and continue to the next screen.
Because this script has not been reviewed by Google, it will generate a warning before you can continue. You must click the "Go to Mailing List (Unsafe)" for the script to have the correct permissions to update your form.

After giving the script the correct permissions,there is an message showes that "Execution completed"
Now your script has the correct permissions to continue to the next step.

### 4. Publish the project

Now your project is ready to publish. Select the `Deploy` button and `New Deployment` from the drop-down.

Click the "Select type" icon and select `Web_app`. 

In the form that appears, select the following options:

- Description: `data list html form` (This can be anything that you want. Just make it descriptive.)
- Web app → Execute As: `Me`
- Web app → Who has access: `Anyone`

Then click `Deploy`.

**Important:** Copy and save the web app URL before moving on to the next step.

### 6. Configure your HTML form

now open the html file and  replacing `YOUR_WEBAPP_URL` with the URL you saved from the previous step.

Now when you submit this form from any location, the data will be saved in the Google Sheet. 🥳