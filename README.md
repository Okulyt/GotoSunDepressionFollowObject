# GotoSunDepressionFollowObject
A Stellarium script allowing to track up to three objects over a sequence of days at a certain sun depression (usually civil twilight). It can plot Mercury visiblity, planetary conjunctions or let you find the best periods of observability for a comet.



Stellarium script to go to specified sun depression, either morning or evening, depending upon variable setting, mark a desired object and follow it for a sequence of days.

Created by expanding GotoSunDepression (credit see below) by Sven Wienstein, June 8, 2025

- Added tracking for second object

- 2026-03-24: Shortened the in-chart labels to just the date to reduce text densitiy / overlapping

- 2026-05-29: Added a third trackable object, added flags showSunMoonDistance1-3 to calculate and output the objects angular distance from moon and sun

GotoSunDepression: by David O'Neil, Aug, 2019. Released to the public domain, for anyone interested. Just leave this 'created by' (or 'originally created by') verbage in the derived work.

To use:
* Set the date via Stellarium's user interface

* Set 'gotoMorning' = true for morning viewing, false for evening

* You might want to change the 'core.wait(0.03);' line to another number, so Stellarium has enough time to process and update before checking new positions.
This is dependent upon your computer's capabilities, since Stellarium does not do things asynchronously for scripting.

* Run the script.

* You can change the year/month/day and Stellarium will automatically update the time to the selected sun depression. Once it is finished getting to the time, the selected object will be re-selected (the cross-hairs will reappear).
// ******************************************************************************************

