README:

Contents:

-Initialization
-Features and Sequence
-Resources and Citations

----Initialization----

    To start off, Run the file "Get_input.xaml"

    The Program will prompt you to input three numeric values. These will be the
    threshold values for the currencies: US Dollar(USD), Indian Rupee(INR) and
    Euro (EUR).

    To update threshold values, simply re-run this file.

    Note: The values you entered must be relative to 1 Canadian Dollar(CAD)
    For Example: An input of 60.5 INR means that the program will check if
    the value of one canadian dollar is greater than or equal to 60.5
    indian rupees.


----Features and Sequence----
   After initiation, a robot will automate the following steps:

    1. Data Entry
        Every hour the automation will use an API to add the current rate of a
        few foreign currencies into an Excel sheet.

    2. Data Comparison
        The next part of the process involves reading the latest data and
        comparing it to preset values inputted by the user during the
        initialization stage.

        Should the new rate of any one of the three currencies be equal to
        higher than the preset rates the program will automatically send out an
        Email.

    3. Automatic Alerts
        An email attached with the updated spreadsheet will be sent to alert the
        client that the currencies have met the threshold.

    4. Backing Up Data to Google Drive
        To prevent data loss, everytime an email is sent the attached Excel file
        is cloned into a Google Sheets file which will be saved on the cloud.

        However, this sheet is only a basic copy and as such the Date and Time
        will not appear on the Google Sheets file.



    Note:
        Changing the Preset Values can be done in one of two ways.
        Either: Repeat the steps from the initialization process.

        or alternatively if facing an error you can:
            1. Open the Excel Sheet where Data Entry occurs
            2. Navigate to "sheet2"
            3. Column A has the currencies and Column B has the preset rates for
               that specific currencies.
            4. Change the inputted values to the desired value.

            Caution:ONLY change the values of the "THRESHOLD" column. In other
            words only edit cells B2, B3 and B4. And ensure the value inputted
            is numeric.

----Resources and Citations----
    API: Free Currency API
        https://freecurrencyapi.net/

    YouTube Videos:
        1. Bogdan Ripa - Scheduling an UiPath unattended processes on your
           development computer
        2. ExpoHub - Uipath Email Automation (Send Emails Dynamically)
        3. Anders Jensen - How to do Real Time Currency Conversion in UiPath
           and Excel - Full Tutorial

    UiPath Forum Posts:
        https://forum.uipath.com/t/job-configuration-not-valid/353029/2
        https://forum.uipath.com/t/how-to-get-the-system-time/18574

    Uipath Docs:
        https://docs.uipath.com/activities/docs/about-the-excel-activities-pack
        https://docs.uipath.com/studio/docs/tutorials
        https://docs.uipath.com/activities/docs/manage-multiple-excel-files

    Zoom Sessions

