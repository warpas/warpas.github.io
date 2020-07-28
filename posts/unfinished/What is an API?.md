# What is an API?
#coding #computing101 #post/in_progress

There are a many ways to interact with computer systems. How often do you think about alternate methods of using your favourite phone app?

 I’d like to bring you closer to one particular method, that most non-programmers don’t usually think about. It happens to be potent in making apps even more useful. It also gives a powerful model for human communication. I’m talking, of course, about APIs. What are those? Well, do I have a treat for you today!

### Interfaces around you

You probably know what a visual User Interface is. One of the simplest UIs you’ve ever seen is the front page of Google Search.

![](What%20is%20an%20API?/google_ui.png)

Just type what you want to find, press “Enter” or click one of two buttons. Interfaces usually strive for simplicity. Your interactions with them come down mostly to clicking, swiping or using the keyboard to type a bit, drag-and-drop elements around and to push buttons on the screen. But I don’t want to dwell on UI design here. Let’s just say the more useful a program tries to be, the more complex the UI gets. You’ve probably come across interfaces like these:

[Blender UI](https://i.redd.it/u9nha9xbudnz.jpg) <change to img tag>
[Link to a thread](https://www.reddit.com/r/computers/comments/71pcgm/post_software_with_the_most_complicated_ui/) with some another daunting examples.

They’re not pretty, but  they get their job done. The more features they brag about, the longer you have to spend on tutorials to know your way around the application.  But fear not! Interfaces can have an even more simplistic look and at the same time be even harder to use for the uninitiated.  I’m talking, of course, about CLI.

Command Line Interface. Anyone who tried to learn programming probably came across this beast at some point. I’m fairly sure it made a bad first impression.

![](What%20is%20an%20API?/Screenshot%202020-06-29%20at%2017.30.02.png)
The command above just lists the contents of a folder. The same thing looks like this in Finder. I’m sure you know how it would look on Windows.

![](What%20is%20an%20API?/Screenshot%202020-06-29%20at%2017.34.21.png)

The simplicity of the Command Line Interface comes from the input method - the keyboard. You can be sure that any type of interaction from the user in that wretched system will be text-based. The only way to interact with it is to just type out commands you want to run. It’s simple if you know the command you want to run. It’s UX hell if you don’t know them.

It does show a very important point though - computers translate your clicks, swipes and button presses to some sort of text, that gets further translated to machine language - ones and zeroes. Whether you type commands using a CLI or click around your windows the results are the same. A command for renaming a file (use an image file)
`mv tumbleweed.gif tumble.gif`
does essentially the same thing as clicking Rename and using `tumble.gif` as the new file name.

CLI used to be the default way to interact with the computer before Windows existed.  It has a higher bar to entry than the UIs of today. Using command line programs required you to at least glance at the documentation or simply “RTFM”. I’m far from teaching you how to use a CLI. The key takeaway here is for you to know something like that exists under the proverbial hood.

### Interfaces on the Internet!

You know how to use Google search. Maybe you don’t use search parameters that often (“kotlin site:blog.duolingo.com”) but that’s a bit too close to CLI territory. You know your way around the web. You can comfortably click/swipe through Wikipedia, Youtube, Facebook, Pinterest, Discord, TickTok or your other favourite websites. Did you know you can also use these sites without having to visit them personally? You could just write a tiny script that does something for you.

**<WE GOT HERE EDITING !!!!!>**

Were you ever in a situation when you wanted to buy tickets to a concert and refreshed the page over and over again in order to get the tickets before they’re all sold out? That’s what a script could do for you. It’s a bit crude, because the script you write technically tries to act like a human controlling the computer’s input methods. It can input text or click on things.

<link to Al Sweigart painting squares with a script>
But there are ways to write scripts that can do much more meaningful actions than clicking or using the keyboard. You can write a script that adds an event to your calendar. It doesn’t have to click around the Google Calendar UI <Insert a GIF of adding a Google Calendar event>
It can do it with just one command. This is where the aforementioned API comes in.

### Apps can talk to each other

Imagine you use Google Calendar to schedule a few video calls for work, and later you need to count the time you spent on those calls and use the total hour count in a monthly invoice that you keep the template for in Google Sheets. You could manually count those hours up . You could then fill your invoice template and be done with it. Done for this month. Then do that again next month. And so on, for every month for the foreseeable future…

There’s also another way. These apps can talk to each other for you. Computers are great at boring, repeatable tasks. You could have a simple script  ask Google Calendar about those events from an entire month. Then it would calculate the hours you need for your invoice. Then send the data to Google Sheets, to the exact template you want. Once you have that script, all you have to do is run it once every month. That could be automated as well.

What I wanted to illustrate with that example is that many of the web applications you use every month can talk to one another. More specifically - you can make them send specific messages between them.  Messages like these:
* “Hey Google Calendar, create a calendar event corresponding with this Toggl time entry”.
* “Hey Twitter, I want you to post on my behalf whenever I publish a video on Youtube”
* “Hey Trello, I want you to create a card in my project whenever I get the email newsletter from my favourite source”.
The only requirement to participate in that conversation is to provide, what nerds call, “a public API”.

### Wait, what are those APIs?

 An API is a different way of communication with the same services. It stands for “application programming interface”. I’ll show you why it has “programming” in the name. Communicating with an application through an API is a bit different to the UI. It’s more precise but with a caveat - it’s more difficult to read for humans. Take a look!

![](What%20is%20an%20API?/google_api.png)

In the example above the green box  contains the request we send to the API endpoint, and the blue box contains the response from the server.  To the untrained eye it’s far from understandable English sentences and closer to math equations or even random strings of characters with some English words thrown in for giggles. The response you get depends on the request you send. Without any prior knowledge it’s difficult to guess what request you should send to get a desired response.

Luckily with popular APIs you don’t have to guess. The example above is based on instructions from [Google’s developer docs](https://developers.google.com/custom-search/v1/using_rest#making_a_request). The documentation specifies what you can expect. “Click here to get the API key”, “send us your key and the search query term and we’ll send you the query result in JSON format”.

API is a precise way of communicating. Once you figure out how a particular API endpoint works, you can rely on it to give you a predictable response. And if you get lost you can always read the docs or rely on trial and error.

### The “I’m not a programmer, I don’t care” section <needs better title>
### In conclusion

You don’t need to be a programmer to take advantage of APIs. There are plenty of programmers who have already written scripts for most of the use cases that interest you. And you can use a lot of existing APIs on you phone with the Shortcuts app (iOS) or Action Blocks (Android). But using APIs by non-programmers is a topic for another time.

There is a different, much more important reason why I took so long talking about APIs today. The model of communication the APIs use (doesn’t matter if it’s REST or GraphQL) is an accurate metaphorical way of thinking about  communication between people. It’s a fascinating topic and I can’t wait to talk about it detail next time!

_No, I’m not shooting for a_ [Wait But Why](https://waitbutwhy.com/) _post length anytime soon._
