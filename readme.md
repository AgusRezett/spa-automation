# SPA Automator

This script automates the process of opening multiple terminals and running specific commands within them, such as starting various microservices or development servers. It's designed to streamline the setup process for development environments.

## Requirements

Before running this script, ensure you have the following installed on your system:

- macOS (The script uses AppleScript and Terminal commands specific to macOS.)
- AppleScript
- Terminal
- Yarn (or modify the script to use your package manager of choice, such as npm)

## Setup

1. **Clone the repository** to your local machine:

   ```sh
   git clone <REPOSITORY URL>
   ```

   Navigate to the script directory (if it's in a specific directory):

   ```sh
   cd <DIRECTORY>
   ```

2. **Open the AppleScript file in Script Editor.**
   Modify the variables at the top of the script (YOUR_USER, MASTER_FOLDER, and PREFIX_SPA) to match your environment and project structure.
   Save your changes.

Running the Script:
To run the script, open the Terminal and execute the following command:

```sh
osascript /path/to/your/script.scpt
```

Replace /path/to/your/script.scpt with the actual path to the AppleScript file.

## Additional Tips

### Converting Script to an App with Automator

For those who prefer a graphical user interface (GUI) or would like to run the script with a simple double-click, you can convert the AppleScript to a standalone application using Automator, a tool available on all macOS computers. This can greatly simplify the process of starting your development environment. Here's how:

1. **Open Automator**: Find Automator in your Applications folder and open it.

2. **Create a New Document**: When prompted, choose to create a new "Application."

3. **Add AppleScript**: Search for the "Run AppleScript" action in the actions library and drag it to the workflow area. Replace the sample script with your own AppleScript code.

4. **Save Your Application**: Go to File > Save, and choose a convenient location to save your new app. Make sure to select "Application" as the file format.

5. **Run Your New App**: Navigate to where you saved your new Automator application and double-click it to run your setup script.

This method provides a more user-friendly way to execute scripts and can be particularly useful for those not comfortable using the terminal or for simplifying repetitive tasks.

Remember, if you modify the original AppleScript, you'll need to update the Automator application with the new script.

## Important Notes

1. **Permissions**: Depending on your macOS security settings, you might need to grant permissions to Terminal or Script Editor to control your computer. This can be done in System Preferences > Security & Privacy > Privacy tab.

2. **Customization**: The script includes placeholders and paths that you'll need to customize based on your project's structure and requirements.

3. **Asynchronous Execution**: The script launches a loading dialog asynchronously, allowing the rest of the script to execute without waiting for the dialog to close.
