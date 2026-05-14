# Astralixi App Library
 
This is the official app library for AstralixiOS. If you made an app and want it to show up in the library on-device, this is the right place.
 
---
 
## What even is this repo
 
So basically this is where all the apps for AstralixiOS live. When someone on Astralixi browses the app library, the apps they see come from here. If your app gets accepted it'll show up for everyone to install which is pretty cool.
 
---
 
## How to submit your app
 
Before you do anything make sure your app actually follows all the rules (see below). If it doesn't it's just gonna get rejected and that's a waste of everyone's time.
 
**Step 1 — Make a GitHub repo for your app**
 
Your repo needs these three files, nothing else really:
 
```
my_app/
├── my_app.py     ← the actual app
├── README.md     ← explain what it does and how to use it
└── LICENSE       ← pick any open source licence, MIT is fine
```
 
Do NOT put `astralixios_api.py` in there. AstralixiOS already has it, you don't need to include it.
 
**Step 2 — Fork this repo and open a pull request**
 
Fork the repo, add your app folder inside `submissions/`, and add an entry for it in `submissions/index.json` with the name, a short description, and what category it is.
 
**Step 3 — Wait**
 
Someone will look at it manually and check everything's good. If something's wrong they'll leave a comment explaining what to fix. Once it passes it gets compiled and added to the library within 24 hours.
 
---
 
## The rules
 
These are hard requirements. Break any of them and your app won't get accepted, no exceptions.
 
**TUI only** — Your app has to run inside the terminal. No separate windows, no tkinter, no pygame, nothing like that. If it opens a window it's an instant no.
 
**Python standard library only** — You can't use pip or any third party packages. Only the stuff that comes with Python by default. This is so the app works on any clean install without any setup.
 
**Use the AstralixiOS API** — You have to import `astralixios_api` and use it for everything. Don't write raw curses code or print ANSI escape codes yourself, the API does all that.
 
**One file only** — The whole app has to be a single `.py` file. No extra modules or folders of code. (This might change in a future version but for now it's a hard rule.)
 
**Show how to quit** — Q and Escape quit automatically but you have to actually show that somewhere on screen, like in the status bar. If the reviewer can't figure out how to close your app it gets rejected.
 
---
 
## What the review checks
 
When someone looks at your submission they're checking:
 
- Does it follow all the rules above
- Does it actually run without crashing
- Does the README actually explain what the app does
- Is the exit option visible somewhere
That's basically it. If everything's fine it gets approved, if not you'll get a comment telling you what's wrong and you can fix it and it'll get looked at again.
 
---
 
## A few other things
 
- Don't submit something that's broken or half finished, actually test it first
- The review is manual so it might take a little while, just be patient
- If your app does something that could be a security issue it will definitely get rejected
- All apps in this library have been verified by Astroxia before they're distributed, that's just how it works for safety reasons

---

*Part of the AstralixiOS project — https://github.com/Astroxia/AstralixiOS*
