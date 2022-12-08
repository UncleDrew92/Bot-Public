# AMC Act-On Bot Classification

This software takes in data from the Act-On Data Studio download template "Bot Classification Template" for any number of specified campaigns/messages and predicts the number of bot vs. legitimate actions.

Initially appeared on
[github](https://github.com/UncleDrew92/AMC-Bot-Filtration).

## Getting Started

These instructions will guide you on how to download the data and run the software that analyzes it

### Prerequisites

Requirements to gather the data
- [Act-On AMC Nurture Login Information](https://www.wrike.com/workspace.htm?acc=3789291&wr=15#folder/515831529/list?filters=&sidePanelItemId=630176163&sortOrder=5&spaceId=534508472&viewId=1183989)

## Downloading the Data

Download the data using the instructions found here: [Act-On Data Studio Reporting Example](https://accessmktg.sharepoint.com/:o:/g/Eme4w1CgSP5Fg3sGKZrxH9ABKlmt0mcbxCK_m318izhQCg?e=NRdu9n)

    Follow steps in the section "Email Bot Classification"

Below is a snapshot of what the data should look like. There will be more information not shown in the screenshot

![Data Snippet.png](Images/Data_Snippet.png)

## Sending Data to the Classifier

1. Navigate to the [Sharepoint Folder](https://accessmktg.sharepoint.com/:u:/g/Ec-udWLcBUVLmIpM0OY_VNkB4aBX5TTPKRTEos27EkyP1w?e=cbNEZy) 
2. Open the Link titled: "Link to Classification Web App"
3. Upload your csv and hit submit
4. The data will automatically download in a zip file after it is processed (give it up to a few minutes if the file is large)
5. If any errors arise, contact andrewd@accessmarketingcompany.com

### Analyzing the Results

Classified_Data.csv

    1. The classification column indicates a predicted bot vs. human action. 1 indicates a predicted human action and 0 indicates a predicted bot action
    2. The index column is the row number from the original csv uploaded
    3. All extra information from the download file is included

High_Level_Data.csv

    1. Produces data for the categories 'Sent' 'Unique Opens' 'Unique Open Rate' 'Unique Clicks' and 'Unique Click Rate'
    2. Separates the data by Message

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
