# Digital A-Z Word Bank App Template

This is the source template for each student's individual app. Do not deploy this template repository itself.

## Create a student's app

1. Create a repository with **Use this template**.
2. In `index.html`, replace `PASTE_BRIDGE_WEB_APP_URL_HERE` with that student's deployed Apps Script Bridge `/exec` URL. This is the only student-specific value in the app.
3. Enable GitHub Pages for the student's repository. Give the student that repository's ordinary Pages URL after testing it. No personal link or connection code is required.

The app reads both vocabulary and the released Day limit through the Bridge. It does not need a published Sheet URL, spreadsheet ID, or discovery URL.

## Bridge setup

Copy `setup/Bridge.gs` into the student's standalone Apps Script project. Replace `PASTE_SPREADSHEET_ID_HERE` with that student's Sheet ID, run `setupBridge`, and deploy the Bridge as a web app. The app requires a Bridge that supports the `days` and `study` actions. If a Bridge was created from an older copy of this template, update its script and deploy a **new version** before using the app.

Set the number of released Days in `Admin Settings!B1` on the student's Sheet. Study and Add & Manage will allow Day 1 through that number. The A-Z Word Bank, Everyday Phrasal Verbs, Business Phrasal Verbs, and Proverbs remain available for study when those tabs exist.

## First-app check

Before distributing a new batch, create one student app and check it on a phone. Confirm both study directions flip correctly, a rating in one direction does not change the other, and Reset Progress affects only the current study set and direction. Ratings from older app versions begin fresh; vocabulary in the Sheet is unaffected.
