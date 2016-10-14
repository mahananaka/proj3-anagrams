# proj3-anagrams
Vocabularly anagrams game for primary school English language learners (ELL).
This project was for the author's CIS322 class during Fall 2016 at the University
of Oregon.

## Author
Jared Paeschke, paeschke@cs.uoregon.edu

## Overview
This anagram game is intended for individuals in the process of learning English.
Most of this game is written in using python and javascript. The bulk of the page
display is done with Flask, Jinj2, CSS. In addition, JQuery, Ajax, and JSon were 
used to design the game without requiring page refreshes.

The user should be unable to type letters that are not in the jumble of letters.
By default once the user finds 3 unique words s/he wins. The world list can be 
changed within the config files. As the user types letters in, the jumble letters 
used are faded out, indicating that they have been used. Further, words that 
don't contain the letters typed are faded in the word list.

## Installation
When writing and testing this program, the test machine was a Raspberry Pi 3 running
Raspian Jesse. This is the best sure fire way that the install will go smoothly. 
However you should have success as long as you have bash and make on your server machine

* git clone https://github.com/mahananaka/proj3-anagrams.git < install directory >
* cd < install directory >
* bash ./configure
* make run

The program should then sit idle and wait for page requests. The default port is
port 5000, to get the main page surf to http://< serverip >:5000/ or if you're on the server
machine http://localhost:5000/. To stop the program at any time use ctrl+c.

## Tests
Several automated test file were written to test the game's underlying framework. 
You can run these tests with the command 'nosetests'. There are currently nose tests
for vocab.py, letterbag.py, and jumble.py.



