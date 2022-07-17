# YouClip - CLI
#### This is the CLI version of my now-not-working-and-poorly-made YouClip app in python.
With youclip you can input a youtube video link or a local video path, a start and end time of the desired clip, wait a few seconds and boom:
you got the clip you wanted.



## Requirements:
* Ideally a linux machine
* python3
* more than 5 working braincells

NOTE: You _can_ use this on windows with some little differences explained below.

## Installation

<b> On a Linux machine: </b>

1 - Clone the git repository:
```
git clone https://github.com/adornerz/youclip-cli.git
```
2 - Change directory to the downloaded folder:
```
cd youclip-cli
```
3 - Install the requirements:
```
pip3 install -r requirements.txt
```
4 - Make youclip an executable:
```
sudo chmod +x ./youclip
```
5 - If you want to use youclip anywhere, copy it to the `/usr/bin` path:
```
sudo cp ./youclip /usr/bin
```
6 - Enjoy by using it with:
```
youclip {usage explained below}
```

<br>
<b> On windows: </b> <br>
Step 1, 2 and 3 are the same as in the linux. <br>
Step 4: remove the first line <br>
Step 5: add the .py extension <br>

*I will make the program globally usable in windows as well, just not today.
## Usage:

Parametres:
```
--url OR -u: Youtube video URL to clip
--local OR -l: Local video path to clip
start time & end time in the format MM:SS

*Only one video at a time!

```

<b> On linux: </b>

For youtube videos: `youclip -u {youtube video URL} MM:SS MM:SS`  <br>
For local videos: `youclip -l {local video path} MM:SS MM:SS` <br>
<br>
Examples: <br>
`youclip -u https://www.youtube.com/watch?v=dQw4w9WgXcQ 01:23 03:17` <br>
`youclip -l ~/Downloads/somevideo.mp4 01:23 03:17` <br>
<br>
<br>

<b> On Windows: </b>
Change directory to the folder where `youclip.py` is located, and use `python .\youclip.py` instead of `youclip` in the commands above. (Temporary solution)


