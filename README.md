progress
========

Filter to display progress.

Originally intended for use to filter the output of bower, eg :

$ bower install |& progress

The default output of bower produced progress lines and scrolls down
the page. This script uses one of the fields and an index, and updates
the corresponding lines accordingly, so you get a sort of table with
the progress as the install progresses.

Requirements
============

You need to install node-terminal and carrier :

$ cd; npm install node-terminal carrier

Tests
=====

Tests are there to run manually. Perhaps I'll get round to automating
them sometime.
