# Quebec VaxiCode Tracker

A simple history tracker for the public JSON file used by Quebec's VaxiCode applications to verify vaccination status.

The most recent version can be found [on the vaxi branch](https://github.com/oceantume/quebec-vaxicode-tracker/blob/vaxi/vaxi.json).

## 📅 Covered period

The tracker starts with the very first public version at the time of release in August 2021. It may be missing some updates done between that time and November 2021, but it will automatically track all new updates done after that point.

## 📖 What's vaxi.json?

The `vaxi.json` file is publicly hosted on the Web and is used by the VaxiCode applications to determine whether the data in a valid QR code is an acceptable vaccination status. For example, it indicates that having two doses of the vaccine is good (green).

Code formatting is done on the file when it's retrieved to make it more readable. Additionally, the two fields `g` and `v` are auotmatically stripped out. These fields represent a date and some metadata on the applications and are not relevant here. 

Parsing the file and explaining its content is beyond the scope of this project. You can try reading the file, JSON is a human-readable format even though most of the content itself is not very friendly.

## ⚖ Intention

This tool has no bad intentions. It simply contains a copy of the publicly hosted file so that its change history can be easily navigated. This gives absolutely no useful information for counterfeiting vaccine proofs because it should simply be a coded representation of the latest accepted vaccination status.

If you work for the Government and think this should not exist, please contact me. My email can be found on my profile page.