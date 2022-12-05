# AMC Act-On Bot Classification

This software takes in data from the Act-On Data Studio download template "Bot Classification Template" for any number of specified campaigns/messages and predicts the number of bot vs. legitimate actions.

Initially appeared on
[github](https://github.com/UncleDrew92/AMC-Bot-Filtration).

## Getting Started

These instructions will guide you on how to download the data and run the software that analyzes it

### Prerequisites

Requirements to gather the data
- [Act-On AMC Nurture Login Information](https://www.wrike.com/workspace.htm?acc=3789291&wr=15#folder/515831529/list?filters=&sidePanelItemId=630176163&sortOrder=5&spaceId=534508472&viewId=1183989)
- [AMC Google Drive Login](https://drive.google.com/drive/)

## Downloading the Data

Download the data using the instructions found here: [Act-On Data Studio Reporting Example](https://accessmktg.sharepoint.com/:o:/g/Eme4w1CgSP5Fg3sGKZrxH9ABKlmt0mcbxCK_m318izhQCg?e=NRdu9n)

    Follow steps in the section "Email Bot Classification"

Below is a snapshot of what the data should look like. There will be more information not shown in the screenshot

![Data Snippet.png](Images/Data_Snippet.png)

## Opening the Software in Google Drive

1. Navigate to the [Sharepoint Folder](https://accessmktg.sharepoint.com/:u:/g/Ec-udWLcBUVLmIpM0OY_VNkB4aBX5TTPKRTEos27EkyP1w?e=cbNEZy) 
2. Download the AMC_Email_Bot_Classifier.ipynb file 
3. Download the "Inputs" folder
4. Upload the file AMC_Email_Bot_Classifier.ipynb to Google Drive and open it (it should say Google Colaboratory)
    - If it does not show up as a Colaboratory file, right-click the file, click open with, and click connect more apps
![Connect Colaboratory.png](Images/Connect_Colaboratory.png)
    - Browse for Colaboratory and install it
    - Right-click the file, click open with, and click Colaboratory
5. Click the folder icon on the left
![Colaboratory Folder.png](Images/Colaboratory_Folder.png)
6. Upload all the files from the "Inputs" folder from Step 1 and the csv file downloaded from Act-On's Data Studio ("sample_data" is irrelevant)
![Colaboratory File Upload.png](Images/Colaboratory_File_Upload.png)
7. Open the File_Name.txt inside and update the name of the file to the name of the csv file making sure to include .csv at the end of the file name
![File Name.png](Images/File_Name.png)
8. Run the program by hitting the play button at the top left or pressing CTRL + ENTER
    - Scroll down to the bottom to see the status of the code. It may take minute or so to run
![Run.png](Images/Run.png)
9. Wait a minute or two until code is done running
10. Click anywhere on the page to see the output file in file folders tab
    1. It may take a few seconds for the files to show up
![img.png](Images/Output.png)
11. Download the output files detailed below 
    1. Hover over the files, hit the ellipses, and click download

### Analyzing the Results

Classified_Data.csv

    1. The classification column indicates a predicted bot vs. human action. 1 indicates a predicted human action and 0 indicates a predicted bot action
    2. The index column is the row number from the original csv uploaded
    3. All extra information from the download file is included

High_Level_Data.csv

    1. Produces data for the categories 'Sent' 'Unique Opens' 'Unique Open Rate' 'Unique Clicks' and 'Unique Click Rate'
    2. Separates the data by Message

## Deployment

In Progress: Uploading to Web App for improved user interface

## Built With

  - [Contributor Covenant](https://www.contributor-covenant.org/) - Used
    for the Code of Conduct
  - [Creative Commons](https://creativecommons.org/) - Used to choose
    the license

## Versioning

We use [Semantic Versioning](http://semver.org/) for versioning. For the versions
available, see the [tags on this
repository](https://github.com/PurpleBooth/a-good-readme-template/tags).

## Authors

  - **Andrew Davis** - *Software Developer* -
    [UncleDrew92](https://github.com/UncleDrew92)

See also the list of
[contributors](https://github.com/PurpleBooth/a-good-readme-template/contributors)
who participated in this project.

## License

This project is licensed under the [CC0 1.0 Universal](LICENSE.md)
Creative Commons License - see the [LICENSE.md](LICENSE.md) file for
details
