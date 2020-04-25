# Whole Foods Autobuy Script

This is a Python script/app that searches for the first available Amazon Whole Foods or Amazon Fresh delivery slot and, optionally, places your order.

## Modifications

This program was modified from the original posted at https://github.com/tangerinehuge/whole-foods-autobuy. Additional notification messages were added. The console "print" statements were uncommented. The chrome options were modified to cache chrome to the user's data directory. The requirements file was modified to install the latest version of each dependency package. This code was executed successfully against an Amazon Fresh cart.

## Installation

**Clone Repo:**
1. Clone the repository to a local directory.
2. Install the necessary modules: `pip3 install -r requirements.txt`
3. Run the script: `python3 WFAutobuy.py`

## Usage
1. Select the refresh interval using the slider (recommend between 20-30 seconds)
2. Uncheck the enable box if you want to complete the purchase manually after a time slot is found.
3. Enable any notifications as desired.
4. Click start to start the search. This will download chromedriver if necessary and then launch a new automated Chrome session.
5. Log in to your Amazon account
6. Add items to your cart if you haven't already.
7. Proceed with the purchase until you reach the time slot selection page.

The script will take over at this point, auto-refreshing at whatever interval you selected. It will select the first open spot when one becomes available and proceed with the purchase.

The first time you run the program it will launch with the default settings enabled. Any changes to the settings will be saved between sessions.

![Config Screenshot](/images/config.png?raw=true "Configuration Window")
