# debugging_javascript_vss
Debugging javascript on Visual Studio

# Debug Node based application
* Click on Add Configuration launch.json will be created under the folder .vscode 
* Then select option {} Node.js: Launch Program
* launch.json will have json element something like below, change the javascript file which wants to be tested under the program
{
  "type": "node",
  "request": "launch",
  "name": "Launch Node Program",
  "program": "${workspacefolder}/app.js"
}

# Debug AVA Tests
* Click on Add Configuration launch.json will be created under the folder .vscode 
* Then select option {} Node.js: Launch Program
* launch.json will have json element something like below, change the javascript file which wants to be tested under args
{
  "type": "node",
  "request": "launch",
  "name": "AVA Tests",
  "program": "${workspacefolder}/node_modules/ava/profile.js",
  "args": [
    "${workspacefolder}/test/test.js"
  ],
  "internalConsoleOptions":  "openOnSessionStart"
}

