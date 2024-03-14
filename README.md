# ovsn
open video social network

# project information
* author: jas387
* version: 0.0.0
* creating data: 2024-14-03 13:58
* license: MIT

# description
* foss tiktok like social network
* using python programming language and flet SDUI framework to make crossplatform ui
* my idea is use nostr protocol to turn it in censorship resitant app.
* maybe if a expert want add tor network to turn it anonymous too.

# observation
* i am not a "real" developer, i'm just a guy with idea and a hobby.
* I might not even be able to finish the project because I'm really a beginner and I know this is a big and complex project. But I'm already grateful if I was able to help someone to continue in this direction.

# what is this ?
with the recent USA news of "we gonna ban tiktok" i think we need a new descentralized social video app that allow us to free, opensource, no "private boxes" or government interference, in resume: freedom of speak.

# goals
## home UI
- [ ] video/image swipe
- [ ] potrait and landscape video mode
- [ ] do not disturb
- [ ] plaback controls
- [ ] profile interactions (icon, view, name, follow)
- [ ] video title
- [ ] video interactions (like, dislike, comment, bookmark, share, landscape rotation, download)
- [ ] search
- [ ] audio interactions (mute, find)
- [ ] inbox
- [ ] friends

## inbox
- [ ] new followers
- [ ] likes
- [ ] comments
- [ ] system notifications

## profile
- [ ] photo
- [ ] video
- [ ] name
- [ ] username
- [ ] bio
- [ ] video space (public, private, bookmark, like)
- [ ] edit profile
- [ ] following
- [ ] followers
- [ ] likes
- [ ] share
- [ ] add friends (suggest accounts, scan, invite)
- [ ] account type (public, private, business)
- [ ] creator tools
- [ ] my qrcode
- [ ] settings
- [ ] upload video


## settings
- [ ] account
- [ ] privacy
- [ ] security
- [ ] balance (lightning address ?)
- [ ] notifications
- [ ] activity center
- [ ] content preferences
- [ ] Adverts (Optional)
- [ ] language and location (optional)
- [ ] offline videos
- [ ] free up space
- [ ] report center
- [ ] support center
- [ ] terms and policies
- [ ] switch account
- [ ] log out
- [ ] clear preferences

## reset preferences
- [ ] algorigthm recommendations

## block and report system
- [ ] username
- [ ] tag
- [ ] text
- [ ] deny list
- [ ] allow list
- [ ] report type (nsfw, unsafe content, age restriction)
- [ ] community/context notes (like twitter)

## buy/seller things
- [ ] send tip to: video, user, comment, music
- [ ] course (playlist)
- [ ] video
- [ ] audio
- [ ] image

## video/image post
- [ ] title
- [ ] lenght (internal)
- [ ] data (Year/Day/Month) (internal)
- [ ] description (text with tags, mentions)
- [ ] location
- [ ] allow comments (privacy-comments, bool: true)
- [ ] visibility (privacy-visibility, bool: public)
- [ ] link
- [ ] price (default: free)

## privacy (default: true)
- [ ] allow comments
- [ ] allow bookmark
- [ ] visibility (public, follower, friends, only you, buyer)



## recommendation algorithm preferences
* any user preferences is stored locally or MAY be cypted (by user) on server or both


## various recommendation algorithm - how to do it in descentralized network ?
- [ ] ring

### ring
* the user post a video/image and the serve store it, server notifies the to a small group (10-100 users) of  and wait interactions.
* if positive interactions (like, watch time, comment, share) then nitifies a bigger group (1.000-2.000), and repeat same step with (2k - 4k), (4k - 8k), (8k - 16k) and so on.



# setup enviroment (create and change to project dir)
```
mkdir -pv ovsn
cd ovsn
```
# clone project to src dir
```
git clone https://github.com/jas387/ovsn.git src/
```
# install dependencies
see how to install flet [dependencies](https://flet.dev/docs/guides/python/getting-started)
install full gstream!
# setup enviroment and activate python virtual enviroment
```
python -m venv venv
./env/bin/activate
```
# install python requirements
```
pip install -r src/requirements.txt
```
# run in desktop (linux)
```
flet run src
```
# troubleshooting
if you are using debian and when run and get libmpv.so.1 not found error, just create a symbolic link of libmpv2 as libmpv.so.1 and it will work:
```
sudo ln -s /usr/lib/x86_64-linux-gnu/libmpv.so.2 /usr/lib/libmpv.so.1
```
