# C-Winform-PLC-Data-Collection
A C# Windows form program to collect array data from plc



This Project will need to be opened in Visual Studio and published so you can make into .exe program.
You will need the libtagplc library if it doesnt transfer for you correctly, can get from nuget manager.
I left unpublished so changes can be made ( like to start automatically if needed, I may add that feature in a checkbox later).
For now it can accomodate up to 8 columns + datetime if wanted.  If your familiar with C# adding some more columns should be easy.

Added the Test PLC file I used ( V32 ).


![IPAddress](https://github.com/user-attachments/assets/2db3da87-c1a7-4f75-a6b1-1a348ac84b32)

Add IP address of PLC and set data collect Interval in milliseconds.


![ArrayName](https://github.com/user-attachments/assets/49c5e823-b005-4295-a662-818ec8942929)

Enter array name ( without trailing index! ) and length, then check if dint or string type.



![FolderStoreage](https://github.com/user-attachments/assets/430f15ad-6153-4f6a-a3c7-2ebbf2af3b79)

Enter FOLDER you want data stored in.


![SetName](https://github.com/user-attachments/assets/3ce30e02-21bb-479d-a817-0b72228e33c3)

You can set the name of the columns if you want.  This will add the column names to the Excel sheet as well.

![Nameisset](https://github.com/user-attachments/assets/cee94d8c-0b7c-4d04-be04-101f1aa0601e)
Name Set example.


![StartLogging](https://github.com/user-attachments/assets/0ccf63fa-2a4c-4190-b784-6f5d4dcb5c81)

Hit Start Logging button, you should see textbox under IP Address say "connected" after your interval time runs.
You should see data populating the gridview now as well.


![Connected](https://github.com/user-attachments/assets/5a39035b-31d3-4f88-9367-adca2d7109f3)


![Datesave](https://github.com/user-attachments/assets/33994524-b63a-4251-be36-a46821404757)



![Datetimecb](https://github.com/user-attachments/assets/3f710463-bb77-4e79-ad15-ec98458c82c8)

The Set last column as date/time will append the date/time to the end of your columns.

![Stoplogging](https://github.com/user-attachments/assets/16eb5fc0-49c8-480e-8811-ceee1f9746c9)

Hit stop logging to stop logging and "connected" should now say "stopped logging"





![datacollectsheet](https://github.com/user-attachments/assets/ea59c2b0-0b7d-4a4c-abe4-95b6aeb34920)
If you go to your folder path you should see an excel file with the days date on it.
If you open it you should see your headers and your data.
