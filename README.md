# Microsoft Graph API Data Pull

This repository contains a Python script that interacts with the Microsoft Graph API to fetch data such as users, licenses, and login information, and exports the data to an Excel file.

## Features
- Fetches user data from a Microsoft Office 365 tenant using Microsoft Graph API.
- Retrieves important information like:
  - Email address
  - Username
  - Assigned licenses
  - Date the user was created
  - Last successful login
- Exports the data into an Excel file for further analysis.
  
## Getting Started

### Prerequisites
To run this project, you need the following:
- A Microsoft Office 365 tenant with API permissions for:
  - `User.Read.All`
  - `Directory.Read.All`
  - `AuditLog.Read.All`
- Python 3.x installed on your machine.
- The following Python packages installed:
  - `msal`
  - `requests`
  - `openpyxl`
  - `python-dotenv`

### API Keys and Secrets
API keys and secrets should **not** be committed to this repository. We are using a `.env` file to keep secrets safe, and this file is excluded from version control via the `.gitignore` file.

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/microsoft-graph-data-pull.git
   cd microsoft-graph-data-pull
