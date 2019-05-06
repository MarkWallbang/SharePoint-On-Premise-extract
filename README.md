# Old SharePoint extractor application

With this application you can extract all lists and document libraries of a SharePoint Site (up to SP2016). Please note that you need to have an account with access to that SahrePoint site!
The application consists of 2 files: 
- The sp_extractor.exe, which is the application itself. You need to simply doublelick this file to start.
- The config.ini. This file is used to specify which SharePoint Site you want to extract. You don't need to touch this file at all, as all the settings will be set in the application itself.
You can NOT download content of a SharePoint Online Site, this is still WIP.

All you need to do is to start the application, and input all the necessary information into the input dialogs. Save your configurations by pressing "Save Configurations", and then click "Extract" to start the extraction. 
You will need to fill in the Login information of your windows user, so that the application can access the SharePoint.

## What is extracted?
Tha application will extract all lists and document libraries on the SharePoint. It will store all meta information and list entries in .csv files. Every list and document library is stored as a separate .csv file. Also, the application will generate a JSON file with all information combined. 

## Configuration
Please find an explanation of all fields you need to fill in.

- Username: Put in your username here.
- Password: Input your password here. 
- SharePoint Server: Fill in the Server URL of the SharePoint you want to extract. Please don't forget to put a '/' sign at the end (e.g.https://example.mycompany.com/)
- SharePoint Site URL: Fill in the URL to the SharePoint Site you want to extract here. This time you don't need the '/' sign at the end. (e.g https://example.mycompany.com/sites/11012646)
- Download Path: Please provide a Systempath here, where you want the extracts to be stored. (e.g. C:\Users\xxxxxx\Downloads )
- Filename: Provide a Name you want the .csv files to have.
- Proxy: If you need to access the internet through a proxy, please provide the proxy URL here. (e.g. "http://proxy.mycompany.com") If you don't need connection through a proxy, you can simply leave this blank.

If you have filled in all the information, please hit SAVE CONFIGURATIONS before you start extracting. Otherwise the applicaiton won't recognize your input. When you open the application for the next time, the last saved configurations will be opened.

## The actual code
You can inspect the code in the folder "Code" in this repository. It's all written in Python, and only requires lightweight libraries like "requests". When you download the .exe file, you don't need any Python interpreter or packages installed. It's all contained in the application. 
