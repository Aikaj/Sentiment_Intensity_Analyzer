The script uses the following libraries:

--> gtts (Google Text-to-Speech) to convert text to speech.

--> speech_recognition to recognize spoken commands

--> os to interact with the operating system

--> re for regular expressions

--> webbrowser to open web pages

--> smtplib to send emails

--> requests to make HTTP requests (for fetching jokes)


1. Functions
The script defines three main functions:

--> talkToMe(audio): converts the input audio text to speech using the system's built-in say command.

--> myCommand(): listens for spoken commands using the microphone, recognizes the speech using Google's speech recognition API, and returns the recognized command 
as a string.

--> assistant(command): executes the recognized command by parsing the input string and performing the corresponding action.

2. Commands

The assistant function recognizes and executes the following commands:

--> open reddit [subreddit]: opens the specified subreddit in the default web browser

--> open website [domain]: opens the specified website in the default web browser

--> what's up: responds with a simple message

--> joke: fetches a random joke from a web API and speaks it out loud

--> email: sends an email to a specific recipient (currently hardcoded to 'John Fisher') with a custom message


3.Main Loop

The script enters an infinite loop, where it continuously listens for spoken commands using myCommand() and executes them using assistant().
