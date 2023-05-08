## How to Run the Cherwell Service Manager API Tool

This tool is a C# Windows Form application that calls the Cherwell Service Manager API to retrieve the status and assigned user name for a given incident ticket ID.

### Prerequisites

Before you can run the tool, you will need the following:

- Visual Studio or another C# development environment
- A Cherwell Service Manager instance with an API authentication token
- The Cherwell API endpoint URL for your instance

### Installation

To install and run the tool, follow these steps:

1. Clone or download the tool's repository to your local machine.
2. Open the solution file (`TicketStatusTool.sln`) in Visual Studio.
3. Replace the `baseUri` and `token` variables in the `btnCheckStatus_Click` method of the `Form1.cs` file with your Cherwell API endpoint URL and authentication token, respectively.
4. Build the solution (`Ctrl+Shift+B`) to ensure that there are no errors or warnings.
5. Run the tool by pressing the `Start` button in Visual Studio (`F5`), or by navigating to the build output directory and running the `TicketStatusTool.exe` file.

### Usage

To use the tool, follow these steps:

1. Enter the ticket ID for the incident you want to check in the `txtTicketId` textbox.
2. Click the `Check Status` button to retrieve the status and assigned user name for the ticket.
3. The results will be displayed in the `lblTicketStatus` label below the text field.

Note: If the tool fails to retrieve the ticket status and assigned user name, an error message will be displayed in the `lblTicketStatus` label.

This tool is provided under the Apache License 2.0 and is intended for educational and informational purposes only. By using this tool, you agree to comply with the terms and conditions of the Apache License 2.0. The author and contributors of this tool do not assume any liability or responsibility for any damages or losses arising from the use of this tool.
