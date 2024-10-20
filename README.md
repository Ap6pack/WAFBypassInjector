# WAFBypassInjector for Burp Suite
A Burpsuite extension to inject random text into request bodies, designed for bypassing WAFs.

## Overview
The "WAFBypassInjector" Burp Suite extension allows users to inject random strings into the request body, effectively testing and bypassing Web Application Firewalls (WAF) by altering payload content dynamically.

## Features
- Insert random text into request bodies.
- Allows users to specify the size of random text in kilobytes.
- Ideal for bypassing WAFs and testing server behavior under various payload sizes.

## How It Works
The extension adds a new option to the context menu when right-clicking inside the HTTP request editor. After selecting "WAFBypassInjector," the user is prompted to specify how many kilobytes of random text to generate. The text is then inserted into the request body.

## Requirements
- Burp Suite (Community or Professional)
- Python 3.x
- Jython (required for Python-based Burp extensions)

## Installation
1. Download and install [Burp Suite](https://portswigger.net/burp/releases).
2. Install [Jython](https://repo1.maven.org/maven2/org/python/jython-standalone/2.7.4/jython-standalone-2.7.4.jar) for running Python-based extensions in Burp Suite.
3. Clone this repository:
   ```bash
   git clone https://github.com/Ap6pack/WAFBypassInjector.git
   ```
4. Load the extension into Burp Suite:
   - Open Burp Suite > Extensions > Add.
   - Select "Python" as the extension type.
   - Browse to the `src/YourExtension.py` file in this repository.

## Usage
1. Right-click inside the HTTP request editor in Burp Suite.
2. Select "WAFBypassInjector."
3. Enter the number of kilobytes (KB) of random text you want to insert.
4. The generated random text will be inserted into the request body.

## Screenshots
![Extention in action](https://github.com/Ap6pack/WAFBypassInjector/blob/main/images/image.gif)

## Contribution and Reporting Issues
If you encounter any bugs or have suggestions for improvements, please report them via the [GitHub issues page](https://github.com/Ap6pack/WAFBypassInjector/issues).

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
