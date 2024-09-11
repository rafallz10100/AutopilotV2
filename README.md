# AutopilotV2

## Description

AutopilotV2 is an application used to generate/import a *.csv file to Intune for the Autopilot Device Preparation process.

## Requirements

- Windows 10/11
- Minimum 3MB of disk space
- Internet access

## How it works?

### Importing a *.csv file containing a serial number into Intune
1. Launch the AutopilotV2 application
2. Select the Import Serial Number button
3. It will check if the Microsoft.Graph.Authentication module is installed. If it is not, its installation will start
4. Provide your credentials
5. If you do not have the appropriate permissions, you can apply for them in Entra ID or consent on behalf of your organization (depending on the permissions)
6. A check will be made to see if the serial number has been imported before.
7. The *.csv file will be imported

#### Example:
![AutopilotV2](https://github.com/user-attachments/assets/4feb9ed5-1338-4b2d-ac11-8caec93a2b6b)



### Generating a *.csv file
#### It is also possible to generate a file without importing to Intune
1. Launch the AutopilotV2 application
2. Select the Export to cav file button
3. The notepad application will open with the generated data
4. The file can be saved to disk or the contents can be copied

#### Example:
![AutopilotV22](https://github.com/user-attachments/assets/1f6d2c4f-07c0-4ffc-b907-b7228800cef6)



### Incompatible system version with Device Preparation process
1. If the system version is not compatible with the Autopilot Device Preparation process, you will be informed about it in the application window:

![image](https://github.com/user-attachments/assets/892b7b49-d5ee-4128-8631-8a452c4ce023)

2. Select Windows Update button
3. The Windows Update system window will appear

![Zrzut ekranu 2024-09-11 090958](https://github.com/user-attachments/assets/c4506c50-bef0-4100-aed4-a2b7b226d2ec)
5. Install updates


## Reporting problems

Bug reports and improvement suggestions are welcome! You can do this by using (https://github.com/rafallz10100/AutopilotV2/issues).

## Status

The project is actively developed and updated.
