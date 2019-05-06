# Old SharePoint extractor application

With this application you can extract all lists and document libraries of a SharePoint Site (e.g. cws7, aws1, etc...). Please note that you need to have access to that SahrePoint site with your account!
The application consists of 2 files: 
- The sp_extractor.exe, which is the application itself. You need to simply doublelick this file to start
- The config.ini. This file is used to specify which SharePoint Site you want to extract. You don't need to touch this file at all.
You can NOT download content of a SharePoint Online Site, this is still WIP.

All you need to do is to start the application, and input all the necessary information into the input dialogs. Save your configurations by pressing "Save Configurations", and then click "Extract" to start the extraction. 
You will need to fill in the Login information of your windows user, so that the application can access the SharePoint.

## What is extracted?
Tha application will extract all lists and document libraries on the SharePoint. It will store all meta information and list entries in .csv files. Every list and document library is stored as a separate .csv file. Also, the application will generate a JSON file with all information combined. 

## Configuration
Please find an explanation of all fields you need to fill in.

- Username: Put in your Windows username here
- Password: Input your Windows password here. 
- SharePoint Server: Fill in the Server URL of the SharePoint you want to extract. Please don't forget to put a '/' sign at the end (e.g.https://cws7.conti.de/)
- SharePoint Site URL: Fill in the URL to the SharePoint Site you want to extract here. This time you don't need the '/' sign at the end. (e.g https://cws7.conti.de/content/11012646)
- Download Path: Please provide a Systempath here, where you want the extracts to be stored. (e.g. C:\Users\xxxxxx\Downloads )
- Filename: Provide a Name you want the .csv files to have.
- Proxy: If you need to access the internet through a proxy, please provide the proxy URL here. (For VVA, it would be "http://cias3basic.conti.de:8080/wpad.dat")

When you open the application for the first time, there will be example entries already filled in to help you. If you have filled in all the information, please hit SAVE CONFIGURATIONS before you start extracting. Otherwise the applicaiton won't recognize your input. When you open the application for the next time, the last saved configurations will be opened.

## In case of errors
If you are facing errors, please contact me directly under simon.boeder@conti.de and provide me your configuration settings (NOT the password of course). Please keep in mind that you can only extract old SharePOint instances with this application (NOT SharePoint Online, this is still WIP).