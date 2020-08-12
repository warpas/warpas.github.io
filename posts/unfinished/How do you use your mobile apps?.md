# How do you use your mobile apps?
- [x] rozdzielić na 3 artykuły
	- [x] Human API (większość już wydzielona, ale komentarz o “powerful model for human communication” nie jest tu potrzebny
	- [x] Historia rozwoju UI
- [x] Zmiana tytułu - ten nie mówi “how to **MAKE** apps talk”. Bardzie “how they do it”
- [x] Editing pass pisania pod konkretnego czytelnika
	- [x] Slabo zdefiniowany czytelnik docelowy - przekaz nie zdaje się być dopasowany do jednego typu czytelnika.
	- [x] Niepotrzebne rozwadnianie przekazu zdaniami o tym, co czytelnik wie albo o czym ten artykul nie jest.
- [ ] Editing pass odsysania tłuszczu z posta
	- [x] Dodać wiadomość z podsumowania na początku, żeby było wiadomo o co chodzi w artykule
	- [x] Wywalić komentarze typu “I’m not going to get into it”. Just don’t get into it
	- [x] Skrócić część o CLI
	- [ ] Usunąć powtórzenia
	- [ ] Zmienić odniesienia do języka w części o API. Zastąpić odniesieniami do formy komunikacji
- [ ] Editing pass “czy dobrze się to czyta”
	- [ ] Nie jestem jeszcze zadowolony ze wstępu
	- [ ] Nie jestem jeszcze zadowolony z sekcji CLI
	- [ ] Przeczytać dalej
- [x] Dodać na końcu coś o “It also gives a powerful model for human communication. “? Nie.

#coding #computing101 #post/in_progress #humanapi

What is your favourite way to use the Google Calendar app? How about other apps? Is your answer “the normal way - on my phone or laptop”? 

Many people who never studied programming don’t know there are other ways. And no, they don’t require learning a programming language. How often do you think about alternate methods of using your favourite phone app?

<Thesis>
Imagine you only communicated with other people by grunting and pointing your fingers. It’s far from enough for having a meaningful exchange of ideas or feelings. But it’s perfect for warning someone about a nearby threat and it’d probably be sufficient to get you food and shelter. It’s a good analogy for using computer systems. There is more than one way to do it. I’d like to expose you to a few methods, that you probably don’t think about that often. Hopefully they’ll shift your perspective of what you can do with your computers, large and small. Let’s get started!

<Talking Points>
### The ones you’re used to - visual interfaces 😎

You’ve seen visual User Interfaces hundreds of times. That’s the main way we interact with technology. One of the simplest example of an UIs is the front page of Google Search.

![](How%20do%20you%20use%20your%20mobile%20apps?/google_ui.png)

Just type what you want to find, press “Enter” or click one of two buttons. Limiting or hiding options is the name of the game here.

- - - -
Some common characteristics of visual UIs are:
* Main design goal - Simplicity - they are designed to be intuitive so that anyone could figure out how to use them on their own
* Input method - You interact with this type of interface primarily with touch screens, mouse and keyboard. Usually in that order of importance.
* Response - The interface responds visually - it redirects you, draws something, flashes or throws a spinner on the screen to ease wait time
* Learning curve - they’re usually easy at the start. The more features they have the more documentation/tutorials they require.
- - - -

The same broad list would apply to the vast majority of GUIs - graphical user interfaces. That would be nerd-speak for your Windows, Mac or Linux applications, as well as phone and tablet apps. Here’s an example:

![](How%20do%20you%20use%20your%20mobile%20apps?/Screenshot%202020-06-29%20at%2017.34.21.png)

 You might not be familiar with it if you’re used to Windows. But it’s similar enough, isn’t it? I’m tempted to talk at length about the other side of the learning curve - the daunting and difficult to understand apps bursting with features. For now, if you’re interested take a look at [this Reddit thread](https://www.reddit.com/r/computers/comments/71pcgm/post_software_with_the_most_complicated_ui/) and check out the Blender UI:

[Blender UI](https://i.redd.it/u9nha9xbudnz.jpg) <change to img tag>

### The text-based world ⌨️

![](How%20do%20you%20use%20your%20mobile%20apps?/Screenshot%202020-06-29%20at%2017.30.02.png)

Command Line Interface. Anyone who tried to learn programming probably came across this beast at some point. I’m fairly sure it made a bad first impression.

This image shows the view of the exact same folder as the Finder GUI image we’ve just looked at.  It’s a bit less obvious and you have to know that in order to see the list of files inside the “Music” folder, you have to type `ls Music`. It’s not written anywhere on the screen, you just have to know. Oh, and it won’t work in the old Windows command line terminal. To get similar output there you need to type `dir Music`. How are you supposed to know that?

- - - -
Some common characteristics of CLIs are:
* Main design goal - They strive to be fast and powerful. All that with the fewest possible inputs.
* Input method - You interact with this type of interface almost exclusively with the keyboard. You can use the mouse but make no mistake - that’s definitely the secondary input device with a CLI.
* Response - The interface responds with text. Luckily the text can have some colour and nowadays emojis are also an option 🥳
* Learning curve -  The basics of CLI use are not intuitive in my opinion. Getting over that initial hump is difficult without a good tutorial, book, mentor or technical manual. Most programs give you access to built-in documentation. The more you know the easier it gets. With enough practice it’s the fastest interface to use for most of your Operating System needs.
- - - -
-The simplicity of the Command Line Interface comes from the input method - the keyboard. You can be sure that any type of interaction from the user in that wretched system will be text-based. The only way to interact with it is to just type out commands you want to run. It’s simple if you know the command you want to run. It’s UX hell if you don’t know them.-

![](How%20do%20you%20use%20your%20mobile%20apps?/Screenshot%202020-08-06%20at%2019.50.34.png)

The emoji in the example above do little to alleviate the pain of learning the ropes with the Command Line. The argument that “it gets better later” is hardly convincing in this day and age. As on British games critic once said about something, that gets good 20 hours in - “You know that’s not really a point in its favour, right? Put your hand on a stove for 20 hours and yeah, you’ll probably stop feeling the pain, but you’ll have done serious damage to yourself.”

However it shows a very important point - computers translate your clicks, swipes and button presses to some sort of text, that gets further translated to machine language - ones and zeroes. Whether you type commands using a CLI or click around your windows the results are the same. A command for renaming a file - `mv tumbleweed.gif tumble.gif` - does essentially the same thing as clicking Rename and using `tumble.gif` as the new file name.

The vast majority of everything you use your computer for with visual interfaces can be done with the command line interface. Let that sink in. 

CLI used to be the default way to interact with the computer before Windows existed.  -It has a higher bar to entry than the UIs of today. Using command line programs required you to at least glance at the documentation. I’m far from teaching you how to use a CLI.- The key takeaway here is for you to know something like that exists under the proverbial hood.

### The method apps use to talk to each other 📲

We’ve arrived at the API or Application Programming Interface, which suggests it’s the one for programmers. But I think the name is misleading. It’s the way applications use to communicate with one another. -You don’t have to understand all of the rules of the language to know the gist of what is being said.- And the meaning behind messages they send is easy to understand. Take a look:

* “Hey Google Search, show me the results for a search for ‘Seattle’.”
* “Hey Google Calendar, give me a list of events scheduled for next Monday in my calendar”.
* “Hey Twitter, I want you to post this message through my user account.”
* “Hey Trello, I want you to create a card in my project and put it in the ‘In Progress’ column.”
* “Hey Toggl, start a timer tagged work”. 
* “Hey Google Calendar, create a calendar event at 9:30 on Thursday”. 

You don’t need a college degree in Computer Science to understand what the responses are going to mean. Sure, the language they are encoded in will be a bit quirky but nobody expected you to read and understand Shakespeare’s Hamlet in its entirety during your first English lesson, right? 

<**GOT HERE IN THE EDITINTG PASS**>

- - - -
Some common characteristics of APIs are:
* Main design goal - to make it possible for various different apps to talk to each other. 
* Input method - text in the format accepted by the API. Details depend on the type of API. But regardless if it’s REST or GraphQL, JSON or XML, you send a message in some type of text format. You can figure out what to send by reading the documentation and monitoring responses to the test messages you send.
* Response - text in a format similar to the input message.
* Learning curve - in many ways they are like CLIs that never get past the “it gets easier now” point. There are some commonalities between APIs that you can learn to recognise and use. But every API is different enough that you can’t skip reading its manual. 
- - - -

We started off with the screenshot of Google Search UI. Let’s take a look at a small example of an API interaction with that service!

![](How%20do%20you%20use%20your%20mobile%20apps?/google_api.png)

There are two messages here:
* The request I sent - in the green box
* The response from the API - in the blue

Those messages aren’t pretty. To the untrained eye it’s far from understandable English sentences and closer to math equations or even random strings of characters with some English words thrown in for giggles. At least at the first glance. But I bet you could understand parts of it. What do you think it does? What service does it access? What did the service respond with? What can you deduce from the URL in the green box? Please take 10-15 seconds to think about it.

The exchange in the example above shows a “Seattle” query to Google Search. The response you get depends on the request you send. Without any prior knowledge it’s difficult to guess what request you should send to get the desired response.

Luckily with popular APIs you don’t have to guess. The example above is based on instructions from [Google’s developer docs](https://developers.google.com/custom-search/v1/using_rest#making_a_request). The documentation specifies what you can expect. “Click here to get the API key”, “send us your key and the search query term and we’ll send you the query result in JSON format”.

API is a precise way of communicating. Once you figure out how a particular API endpoint works, you can rely on it to give you a predictable response. And if you get lost you can always read the docs or rely on trial and error.

### In conclusion

You’ve seen a few types of interfaces by now. They were sorted from the most intuitive visual UIs to the least intuitive APIs. The text based UIs seem to have a steeper barrier to entry and require reading documentation for basic usage. Technical manuals rarely are an invigorating read. When you want to tell your application to do something you can use either one of these interfaces.

You can tell Google Calendar to add an event on Friday at 11:00 AM in many ways:
* Click around in the browser on a laptop or desktop computer
* Touch and swipe in the mobile app on a phone or tablet
* Use one the many Command Line interfaces
* Have Apple Calendar copy it through an API integration

The end result is still the same - there will be an event on Friday at 11:00 AM in your Google Calendar. If there’s one key takeaway I have for you here, it’s this - there is more than one way to interact with computer systems.

All of these interfaces are akin to different languages you can use to talk to computer systems.

These methods are much like different ways to communicate with people. Imagine if you only 

there is more than one way to interact with computer systems. All of these interfaces are akin to different languages you can use to talk to computer systems. 

<Call to Action>

Thank you for reading! ❤️

_No, I’m not shooting for a_ [Wait But Why](https://waitbutwhy.com/) _post length anytime soon._