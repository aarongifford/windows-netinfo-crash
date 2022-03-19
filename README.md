# windows-netinfo-crash
React Native Windows netinfo crash sample

To run the app on windows use these instructions: https://microsoft.github.io/react-native-windows/docs/getting-started#running-a-react-native-windows-app

**Without Using Visual Studio**

In your React Native Windows project directory, run:

npx react-native run-windows

📋
Copy
For information on the options that @react-native-windows/cli takes see React Native Windows CLI.

A new Command Prompt window will open with the React packager as well as a react-native-windows app. This step may take a while during first run since it involves building the entire project and all dependencies. You can now start developing! :tada:

**Using Visual Studio**

From the root of the project directory, run the following script which will automatically link your app's dependencies:
npx react-native autolink-windows

📋
Copy
Open the solution file in the application folder in Visual Studio (e.g., AwesomeProject/windows/AwesomeProject.sln if you used AwesomeProject as <projectName>)
Select the Debug configuration and the x64 platform from the combo box controls to the left of the Run button and underneath the Team and Tools menu item.
Run yarn start (or npm start) from your project directory, and wait for the React Native packager to report success.
Click the Run button to the right of the platform combo box control in VS, or select the Debug->Start without Debugging menu item. You now see your new app and Chrome should have loaded http://localhost:8081/debugger-ui/ in a new tab. Press F12 or Ctrl+Shift+I in Chrome to open its Developer Tools. :tada:
  
**To replicate the 5G crash**
1) Install the application on a device that has a 5G modem and SIM card
2) Set up the 5G connection
3) Disconnect the device from 5G and LAN internet
4) Start the sample application
5) Connect the 5G internet
