# Dropbox-Share-URL

This is a folder action script that automatically takes the dropbox share URL for the most recently added single file, creates a bit.ly link from it (using your bit.ly account) and sends the shortened URL to your clipboard.

## Why This Script
I sought out to create this (based on found scripts, see 'Acknowledgements' below) as I've been using dropbox as an alternative to Drop.lr/Cloud App for some time. I got tired of manually having to find the file I wanted to share, right clicking, copying the public link and then creating a shortened bit.ly link out of it. This script now saves me a ton of time.

## How to Use

1. Launch AppleScript and open the script file you downloaded for GIT.
2. Insert your **Bit.ly Information**. Put a username and API key in the 2 properties: login, api_key [bit.ly name and API key page](https://bitly.com/a/your_api_key/)
3. Insert your **Dropbox Information**. The number that shows up in the URL of your public links when you select “Copy Public Link.” So, if the URL to a file called “untitled.jpg” looks like this: http://dl.getdropbox.com/u/123456/untitled.jpg, then you should replace “userid” with “123456”. This script assumes you're using a subfolder within your Public folder director. No need to include the trailing slash, just the folder name.
3. Save the script as “DropboxShareURL.scpt”
4. Put the script in the folder: Macintosh HD/Library/Scripts/Folder Action Scripts
5. Right-click on your Public Dropbox folder and select “Folder Actions Setup…”
6. The “Folder Actions Setup” application should open and should immediately allow you to “Choose a Script to Attach”
7. Click on “DropboxShareURL.scpt”
8. Click the checkbox to “Enable Folder Actions”.

Each time you drop a single file into this folder (in my case it is called 'shares') the script will run and the results should be a bit.ly URL in your clipboard that links to the dropbox file. If you have Growl installed you will also get a notification.

## Acknowledgements 

This script has been upon the scripts provided by Chez Moncef - [“AppleScript to Automatically Copy Dropbox Public Link to Clipboard When a New File Is Added”](http://chezmoncef.com/post/5496496542/applescript-to-automatically-copy-dropbox-public-link) and Quicksilver Wiki - [Shorten URL (AppleScript)](http://qsapp.com/wiki/Shorten_URL_(AppleScript)).

## Warning

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.