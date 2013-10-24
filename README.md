progress
========

Filter to display progress.

Originally intended for use to filter the output of bower, eg :

$ bower install |& progress

The default output of bower produced progress lines and scrolls down
the page. This script uses one of the fields and an index, and updates
the corresponding lines accordingly, so you get a sort of table with
the progress as the install progresses.

Usage :

$ progress {-f [field index]}

The field index is the index of the field that is unique for lines that
are considered the same entity. The indeces start at 0.

If no field index is supplied, the script guesses from the first column on
the first line - if it is 'npm' then the field index is '3', and if it is
'bower' then the field index is '1', otherwise the field index is '1'.

Requirements
============

You need to install optimist, node-terminal and carrier :

$ cd; npm install optimist node-terminal carrier

Tests
=====

Tests are there to run manually. Perhaps I'll get round to automating
them sometime.
