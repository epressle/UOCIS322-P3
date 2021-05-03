# UOCIS322 - Project 3 - Ethan Pressley, epressle@uoregon.edu #
A vocabulary anagrams game for primary school English Language Learners (ELL) that uses AJAX and Flask to update per keystroke.

NOTE: This project requires Docker.

## Overview

A simple anagram game designed for English-language learning students in elementary and middle school. Students are presented with a list of vocabulary words (taken from a text file) and an anagram. The anagram is a jumble of some number of vocabulary words, randomly chosen. Students attempt to type words that can be created from the jumble. When a matching word is typed, it is added to a list of solved words.

The vocabulary word list is fixed for one invocation of the server, so multiple students connected to the same server will see the same vocabulary list but may have different anagrams.

## Getting started

* Build the simple flask app image using

  ```
  docker build -t your-name-cis322-3 .
  ```
* Run the container using

  ```
  docker run -d -p <someport>:5000 your-name-cis322-3
  ```
NOTE: Make sure to specify a free port for ```<someport>```.

* Launch `http://hostname:<someport>` using your web browser and it the game should display.

* Stop the container using

  ```
  docker stop <container-ID>
  ```
