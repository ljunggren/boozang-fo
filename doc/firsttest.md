Creating your first test
============


Window aligment
------------
In order to use Boozang well, we recommend aligning the Boozang tool and your application next to each other side by side in the following way

![example image](images/settings_general.png "An exemplary image")

This allows you to get a good overview of the recorded actions, and an easy way to modify or delete recorded actions.

The Boozang recorder
------------
Boozang works within the browser which allows for a very stable recording function. Simply click on the record button in the tool. As you perfrom actions on your web page actions will be recorded. To remove an un-wanted action that was recorded simply press the trashbin next to the action in the main tool view. 

Test playback
-------------
As soon as a test has been created you can use the playback button to replay the test steps. Boozang supports 3 different playback modes: Normal, demo and debug mode. Demo mode slows down the playback speed and annotates every test step. This is good for demos and when trying to understand a test that someone else has authored. Debug mode is a very powerful functionality that plays the test, but when encountering an error it highlight the error and allows you to correct it on the fly. When you have corrected the error simple press the play button again and the test will continue it´s execution. This is very useful when updating a test after a big code change. 

Saving a test
-------------
A test is automatically saved in the local storage of the browser. As soon as you update a test, the test will be checked out by you, and it will appear as locked for your team-mates, which prevents them from making changes. As soon as you click save the test will be saved on the Boozang server, and the lock will be automatically removed, allowing other team-members to make changes. 

Creating a validation
---------------
It's also very easy to create a validation, or assertion. Simply click on the validation button and click the element you want to validate in your application. The default validation condition is "exists", that creates an assertion equals condition on the element. You can change the validation condition can be changed in the main tool window. 

Generate test instruction
---------------
Based on your recorded test you can also generate the test steps in clear text format, in our Boozang syntax. Simply click on the magic wand, select "From Actions to generate test case description" and the test instructions will be generated automatically. 

Playback test instruction
---------------
In order to playback the test based on the test instruction you will again use the magic wand. Click on "From test case description to generate actions" and the test case will run, automatically generating test actions. 