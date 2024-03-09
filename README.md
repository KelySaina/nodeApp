
```markdown
# Project Setup Script

## Purpose
This script automates the setup process for a Node.js project with an Express server using CORS, dotenv, and a specified database package. It also includes the installation of nodemon for automatic server restarts during development.

## Usage

### Prerequisites
- Node.js installed on your machine
- npm (Node Package Manager) installed

### Running the Script
1. Open a terminal.
2. Navigate to the directory where the script is located.
3. Run the script with the following command:

```bash
./nodeApp <project_directory> <database_package> [port]
```

- `<project_directory>`: The desired name for your project directory.
- `<database_package>`: The name of the npm package for your chosen database (e.g., mongodb, mysql).
- `[port]` (Optional): The port on which the Express server will run. If not provided, the default is set to 5000.

### Example
```bash
./nodeApp my_project mongodb 8080
```

## Project Structure
- The script will create a new directory for your project, or an alternative with a random ID if the specified directory already exists.
- It initializes npm and installs the necessary dependencies, including express, cors, dotenv, and the specified database package.
- A `.env` file with the specified port is created.
- An `index.js` file is generated with a basic Express server setup.
- The script attempts to open the project in Visual Studio Code, Sublime Text, or Mousepad.
- Finally, it launches the server using nodemon.

## Notes
- If you encounter any issues or errors during setup, refer to the error messages for guidance.
- If no supported code editors are found, the script will provide a message to open the project manually.

## Setup as a Command in Linux
To make this script easily accessible as a command in Linux, you can follow these steps:

1. Make the script executable:

```bash
chmod +x nodeApp
```

2. Move the script to `/usr/local/bin`:

```bash
sudo mv nodeApp /usr/local/bin
```

Now, you can run the script from any terminal window by typing:

```bash
nodeApp <project_directory> <database_package> [port]
```

Note: You may need to use `sudo` for the `mv` command if you encounter permission issues.

```
