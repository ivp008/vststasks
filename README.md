# VSTS Tasks for Azure Automation
Visual Studio Team Services tasks for integrating with Azure Automation

## To build this extension on your machine and upload it privately to your VSTS account for testing:

1. Clone this GitHub repository
1. Navigate to the directory the repository was cloned into on your machine via Command Prompt
1. Via a Command Prompt window, run 'npm install' to install all Node.js dependencies
1. You will also need to install the 'TFS Cross Platform Command Line Interface' (tfx-cli) to package your extension. tfx-cli can be installed using npm by running 'npm i -g tfx-cli'
1. In the 'vss-extension.json' file, enter your VSTS account name as the value for the "publisher" property
1. In the Command Prompt window, run 'tfx extension create'
1. Running the above command will generate a .vsix file
1. Navigate to 'Publish extensions' under 'Browse Marketplace' through VSTS
1. Click the '+ New extension' option and you will be prompted to upload to a .vsix file. Upload the .vsix file generated by building your extension earlier
1. A private version of this extension should now be uploaded to your VSTS account
1. In order to use/test the extension, you must share it with your VSTS account
