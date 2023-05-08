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
