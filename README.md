# Python Instagram Bot
First off this bot was a learning experience for me. I do not intend for people to use this as there is a possibility you will get banned. If that happens I am not responsible. This is a "use at your own risk" kind of software.

## Installation
First you will need to download this repository. After you do that you need to install selenium. Open a new terminal session and run:
```
  > pip install selenium
```
After you have installed selenium you now need to install your browser driver. Different webbrowsers have different drivers. I have included the chromedriver that you need to run this with Google Chrome. If you prefer to use a different browser download and install the driver following the instructions using one of the links below.  
* [FireFox](https://github.com/mozilla/geckodriver/releases)
* [Edge](https://developer.microsoft.com/en-us/microsoft-edge/tools/webdriver/)

After you do that you will need to make sure you use that driver. The bot is pre-programmed to use the Google Driver. If you wish to use a different browser you need to follow the instructions below.  

### FireFox
Open the python script (main.py) using any text editor. Then you need to find line 20 and change
```
self.driver = webdriver.Chrome("./chromedriver")
```
to
```
self.driver = webdriver.FireFox()
```
Save the file and run the program. It should open a new FireFox window and start working.

### Edge
Open the python script (main.py) using any text editor. Then you need to find line 20 and change
```
self.driver = webdriver.Chrome("./chromedriver")
```
to
```
self.driver = webdriver.Ie()
```
Save the file and run the program. It should open a new Edge window and start working.

## What Now
After you get it up and running you simply have to sit back and let it run. Go get a pizza or hang out with friends for once. You no longer need to waste your life away liking Instagram photos because you have a bot to do it for you! I **DO NOT** recommend using this on your main account as there is a chance you will get banned.

## Change the Tags
To change the tags the bot looks up and likes photos from you need to open the python script (main.py) in any text editor and find the tags variable near the bottom of the page:
```
hastags = [...]
```
Change each hastag you want and add more or remove some if you need. Just be sure to keep them all in quotation marks and be sure to separate each new tag with a comma like so:
```
hastags = ["hastag1", "hastag2", ...]
```
Now you have your own custom list of hastags that the bot will use.
