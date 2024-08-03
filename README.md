# J.P. Morgan Chase software engineering program. Task 3

## Starter repo and setting up dev environment
###
    Fork and clone the repo for task 3 of JPMC's Forage program: https://github.com/theforage/forage-jpmc-swe-task-3
    Remember to uncheck the “Copy the main branch only” box in the fork dialog on GitHub. 

    Create a new virtual environment in the project root. e.g. by using the venv module in Python:
    $python -m venv venv 
    This will create a new directory named venv in your project root, containing the virtual environment.

    Activate the Virtual Environment (windows  /  linux):
    $.\venv\Scripts\activate     /     $source venv/bin/activate

    Install all project dependencies. These are listed in the requirements.txt file:
    $pip install -r datafeed/requirements.txt

    Use npm, to install a series of javascript dependencies to your machine. If you already have access to npm on your system, you can skip this step. Otherwise, follow the instructions here (npm comes bundled with nodejs): https://nodejs.dev/en/learn/how-to-install-nodejs/
    For this project to work, you must have node 18.10.0 installed on your machine. Ensure you have the correct version by running “node -v” in your terminal. If you do not, consider using nvm to install the correct version for you.

    Install the necessary dependencies by running `npm install` from the project repo
    $npm install


## The objective (already completed)
Use perspective to generate a live graph that displays the data feed in a clear and visually appealing way for traders to monitor.

Recall that the purpose of this graph is to monitor and determine when a trading opportunity may arise as a result of the temporary weakening of a correlation between two stock prices. Given this graph, the trader should be able to quickly and easily notice when the ratio moves too far from the average historical correlation. Assume that threshold is +/-5% of the 12-month historical average ratio.

## To run 
###
    First, start the python server from the root of the project repo:
    $python datafeed/server3.py

    Next, open a new terminal and start the client by running:
    $npm start

    If your browser window didn't pop up, navigate to:
    http://localhost:3000/