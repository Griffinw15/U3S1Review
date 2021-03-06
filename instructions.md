# Data Science U3S1 Review

In this review you are taking the roll of an inventory manager for a computer shop. All code should be done in .py files to best represent how you will turn in your work on the Sprint Challenge. This review is designed based on the Challenge, but does not give as much detail in the instructions.  This folder includes comps.py with the classes described already completed and comps_test.py with the unit tests to check your work. If you just copy the code out of those files it will defeat the purpose of the review.


## Part 1: Set Up the Data Structure

While working in inventory management you've decided to use some object oriented programming. All the computers you sell have the same basic properties:
- amount of ram
- processor speed
- storage volume
- storage type
- whether or not the computer is on (All computers in your shop are off at purchase)

Write a python class that takes in these values and saves them inside of the object.

Add code to the end of your .py file to run it as a script and test that your attributes are correctly being saved.

## Part 2: Lets Get Computing

Computers stats are nice, but we really want to be able to turn them on to do anything. Write two methods:
- checks the type of storage and if its an SSD returns 'about 10 seconds' or 'time to go get coffee' otherwise. Stretch: raise a ValueError if the drive isn't a legal type (SSD or HDD)
- Checks to see if the computer is turned on, and if it isn't calls the function above to estimate how long until its read to go (and 'turns the computer on')

Adapt your scripting code to check that the new methods also work

## Part 3: But what about the laptops?

Laptops are their own beast! They are similar to base computers but with some additional attributes.

Create a subclass of the Computer you already made and add:
- weight
- make the default type of storage SSD
- add an attribute for whether or not the clamshell is open- all of your laptops start closed.

Additionally, you're going to need some changes to the methods:
- now you'll need to check that the clamshell is open before you turn on the computer
- create a method to open the clamshell

Stretch: add a *property* which determines the portability based on the weight of the laptop. Should return 'very portable', 'a little portable', and 'not really portable'. Use your judgement to choose what weight thresholds to use for these categories.


Again, adapt your script to check the new class and methods.

## General Stretch
There are lots of functions that a computer can do, add additional methods that make sense for a computer. Some ideas include:
- turn off
- run a game
- close laptop

## Part 4: Tests for Days
Now, all that python scripting for tests was great, but in production we need to check programatically that everything is working correctly. Create a test file and create a few functions for testing.

This is an area where you can really use your imagination, anything you can test about your computer you should. The answers do tests about:
- boot time response is correct
- stats are stored appropriately
- laptops can be turned on and opened

## Part 5: Make it pretty
Hopefully as you've been coding you have been paying attention to the pep8 style guides, however if not now is the time to go back and check them. Throw your code through an automatic checker to make sure that its compliant. Additionally make sure that your code is well documented and easy to read.
