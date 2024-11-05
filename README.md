# Python-Port-Scanner
A simple multi-threaded port scanner in Python
Here's a sample README content for your GitHub repository. This README provides a brief description, installation instructions, usage guide, and some additional information on how the script works.

## Features
- Multi-threaded scanning for faster results
- Supports scanning all ports from 1 to 65535
- Error handling for socket-related exceptions
- Easy to use command-line interface

## Requirements
- Python 3.x

## Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-username/python-port-scanner.git
   ```

2. **Navigate to the project directory:**
   ```bash
   cd python-port-scanner
   ```

3. **Install necessary packages** (if any):
   This script uses standard libraries, so no additional installation is required.

## Usage

To run the port scanner, open a terminal and execute the following command:

```bash
python scanner.py <target>
```

- Replace `<target>` with the IP address or domain name you want to scan.

### Example
```bash
python scanner.py 192.168.1.1
```

## How It Works
- The script first validates the target IP or hostname.
- For each port in the range 1-65535, it initiates a socket connection using multi-threading.
- If a connection to a port is successful, it prints that the port is open.
- Each thread runs independently, allowing multiple ports to be scanned simultaneously, which speeds up the process.

## Important Notes
- **Permissions**: Running a port scan against a target without permission may be illegal. Only scan networks and systems you have permission to test.
- **Interrupting the Scan**: You can stop the scan at any time by pressing `Ctrl + C`.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

