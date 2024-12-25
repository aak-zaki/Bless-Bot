# Bless Network Bot

This script automates network or node operations for Blockless Bless Network Bot.

## Register Bless Network

- https://bless.network/dashboard?ref=7C8B9X

## Features
- **Automated node interaction**

## Installation

1. Clone the repository to your local machine:
   ```bash
   git clone https://github.com/aak-zaki/Bless-Bot.git
   ```
2. Navigate to the project directory:
   ```bash
   cd Bless-Bot
   ```
3. Install the necessary dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Run:
   ```bash
   python3 run.py
   ```

## Usage
1. Register to blockless bless network account first. If you don't have one, you can register [here](https://bless.network/dashboard?ref=A759PU).
2. Set and modify `user.txt`. Below is how to set up this file. Put your `B7S_AUTH_TOKEN` in the text file, as shown below:
   ```
   eyJhbGcixxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
   ```
   To get your token, follow these steps:
   - Log in to your Grass account at `https://bless.network/dashboard`.
   - Open developer tools in your browser (press F12 or right-click > Inspect Element).
   - Go to the Application tab, look for Local Storage in the storage list, and click `https://bless.network`. You will see your `B7S_AUTH_TOKEN`.
   - Alternatively, you can go to the Console tab and paste this:
     ```bash
     localStorage.getItem('B7S_AUTH_TOKEN')
     ```
3. Set and modify `id.txt`. Below is how to set up this file. Put your `nodeid(pubkey)` and `hardwareid` in the text file with this format `nodeid(pubkey):hardwareid`, as shown below:
   ```
   12D3Koxxxxxxxxxxxxxxx:e938610xxxxxxxxxxxx
   ```
   To get your token, follow these steps:
   - Download the [extension](https://chromewebstore.google.com/detail/bless/pljbjcehnhcnofmkdbjolghdcjnmekia).
   - Open `chrome://extensions/?id=pljbjcehnhcnofmkdbjolghdcjnmekia`.
   - Enable `Developer mode` in the top right corner, then press `service worker`. A new tab will open.
   - Go to the `Network` tab, open the `Bless extension`, and log in to your account.
   - After logging in, search for a name matching your pubkey (e.g., `12D3xxxx`), open it, and copy the `pubkey` and `hardwareid`.
   
4. Run the script:
   ```bash
   python3 run.py
   ```

**NOTE:**
- The total time is refreshed every 10 minutes of connection.
- Each account can have a maximum of 5 node IDs, which cannot be deleted. It is recommended to save your Node ID (pubkey) and hardware ID.

