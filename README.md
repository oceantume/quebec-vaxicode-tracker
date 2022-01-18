# Quebec VaxiCode Tracker

A simple history tracker for the public JSON files used by Quebec's VaxiCode applications to verify vaccination status.

The most recent files can be found [on the vaxi branch](https://github.com/oceantume/quebec-vaxicode-tracker/tree/vaxi).

## 📅 Covered period

The tracker starts with the very first public version at the time of release in August 2021. It may be missing some updates done between that time and November 2021, but it will automatically track all new updates done after that point.

## 📘 What's vaxi.json?

The [vaxi.json](https://github.com/oceantume/quebec-vaxicode-tracker/blob/vaxi/vaxi.json) file is publicly hosted on the Web and is used by the VaxiCode applications to determine whether the data in a valid QR code is an acceptable vaccination status. For example, it indicates that having two doses of the vaccine is good (green).

Code formatting is done on the file when it's retrieved to make it more readable and the two fields `g` and `v` are automatically stripped out. These fields contain a timestamp and some metadata on the applications and are not relevant here.

Parsing the file and explaining its content is beyond the scope of this project. You can try reading the file, JSON is a human-readable format even though most of the content itself is not very friendly.

## 📗 What's trust-vaxicode.json?

The [trust-vaxicode.json](https://github.com/oceantume/quebec-vaxicode-tracker/blob/vaxi/trust-vaxicode.json) file is also publicly hosted on the Web and used by the VaxiCode application. It contains a list of trusted identities and their associated public keys that are valid to verify signed QR codes. For example, it contains the public keys used to verify that a QR code was emitted by the government of Quebec. It also contains many keys from many entities across the world who are part of the [CommonTrust Network](https://www.commontrustnetwork.org/) registry.

Code formatting is done on the file when it's retrieved to make it more readable and the timestamp field `d` is automatically stripped out.

## ⚖ Legal stuff

This repository was not meant with bad intentions. It simply contains a copy of the publicly hosted file so that the change history can easily be navigated. This gives absolutely no useful information for counterfeiting vaccine proofs because it should simply be a coded representation of the latest accepted vaccination status along with public keys which can't be used to sign vaccine proofs.

I am in no way associated with the Government of Quebec or the people who make VaxiCode. This is my own personal effort and has nothing to do with the company I work for either.

If you work for the Government and think this should not exist, please contact me. My email can be found on my profile page.
