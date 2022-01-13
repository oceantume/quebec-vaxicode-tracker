# Quebec VaxiCode Tracker

A simple history tracker for the public JSON file used by Quebec's VaxiCode applications to verify vaccination status.

The most recent version can be found [on the vaxi branch](https://github.com/oceantume/quebec-vaxicode-tracker/blob/vaxi/vaxi.json).

## 📅 Covered period

The tracker starts with the very first public version at the time of the release in October 2021, but it's missing all updates between that point and January 2022. However, it should be able to track all new updates from that point onward.

## 📖 What's vaxi.json?

This file is publicly hosted on the Web and is used by the VaxiCode applications to establish whether the data in a valid QR code is an acceptable vaccination status. For example, it indicates that having two doses of the vaccine is good (green).

Parsing the file and explaining its exact content is beyond the scope of this project. You can try reading the file, JSON is a human-readable format even though most of the content itself is not very friendly.

## ⚖ Intention

This tool has no ill intents. It simply contains a copy of the publicly hosted file so that its change history can be easily navigated. This gives absolutely no useful information for counterfeiting vaccine proofs because the code should be a coded representation of the latest accepted vaccination status.

If you work for the Government and think this should not exist, please contact me. My email can be found on my profile page.
