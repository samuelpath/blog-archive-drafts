![Emilien Pecoul giving a talk on Domain Driven Design](http://www.samuelpath.com/wp-content/uploads/2017/05/emilien-pecoul-e1494182671839.jpg)

A few months ago, I started a series on Clean Code. After [introducing the series](http://www.samuelpath.com/what-is-clean-code/) by sharing quotes from leaders in the tech industry, I had the privilege of having two friends of mine working at Mozilla share their answers to the question: "What is Clean Code for you?" [Jan](http://www.samuelpath.com/jan/)'s and [Ben](http://www.samuelpath.com/ben/)'s).

One thing I appreciate in this series is how each answer is at the same time unique, yet shares the same fundamental values. Each developer has their own perspective on what makes clean code, yet all essentially agree. It's like watching the same diamond from various angles.

Today, I have the joy of sharing the answer of someone who has had a great influence on my young software development career: Emilien Pecoul.

<!--more-->

We met at the November 2016 edition of the [Fhacktory](http://www.fhacktory.com/) hackathon in Lyon, where the picture below was taken (you can see my back – I'm on the table on the left, in the middle between two teammates while the third one was taking a 3AM nap):

![fhacktory hackathon panorama](http://www.samuelpath.com/wp-content/uploads/2017/05/fhacktory-hackathon-panorama-e1494183444590.jpg)

During our first discussion, I felt his passion to write good software. At the time, I wasn't yet working as a software engineer in my current company, but was coding a lot at home. I developed side projects by myself to improve my development skills (I'll talk about them in another post). The downside to working all by myself – and I didn't realize it at the time – was that I was mostly focusing on making my projects *work* with little to no regard for how clean or tested my code was. As soon as I had a working solution, I moved to the next project.

By discussing with Emilien, I came to realize that even though any piece software obviously had to "work" to be of any use, it was far from enough. Any decent developer can find ways to solve most business problems. But what separates merely *decent* from *excellent* developers is how robust, clean, readable and maintainable their code is.

Clearly, I was well on my way then to become a decent developer, but pretty off-track to become an excellent one. As I got back home after the hackathon, I could not continue to code like before. I decided to follow [Emilien on Twitter](https://twitter.com/Ouarzy), to subscribe to his [tech blog](http://www.ouarzy.com/), and started to ask him a lot of questions by email about clean coding practices.

He's been very supportive and encouraging and has always taken the time to answer. His motto is: "To become a software craftsman, or die in the attempt", and I've witnessed that this is not simply a nice way to market himself, but his core philosophy (why else would he take the time to answer huge emails from a random junior developer?).

Since then, I've seen him many times at various meetups [Microsoft User Group (MUG)](https://www.meetup.com/fr-FR/MUGLyon/), [AlterCoding](https://www.altercoding.com/) or [Human Talks](https://www.meetup.com/fr-FR/HumanTalks-Lyon/) and conferences (like [MiXiT](http://www.samuelpath.com/mixit/) where he's very involved, and each time I've talked to him, I've been inspired in my software craftsmanship journey.

Alright, enough presentation. Let's talk business. Here is his answer to the question: "What is Clean code for you?":

> Clean code has an important meaning for me, because it brings me back to 2010, when I started to understand how ignorant I was.

> For me, [Clean Code](https://www.amazon.com/Clean-Code-Handbook-Software-Craftsmanship/dp/0132350882) is also the title of one of the books that changed my career (the other one is [The Passionate Programmer](https://www.amazon.com/Passionate-Programmer-Creating-Remarkable-Development-ebook/dp/B00AYQNR5U/)).

> I guess it was not exactly the answer you expected, but it’s really what Clean Code is for me. Because following the practices described in this book, day after day, helped me to learn more and to take pride in the code I ship.

> When I understood that it was actually possible, despite the fact that most people were telling me that "tests are too expensive" or "comments are mandatory for maintenance", it changed the way I worked. I quickly realized that I delivered much more value than before for my customers, and because the company I was working for was not really aware of these practices, I quit my job and started a career as a freelance.

> My new mantra has been ever since: I will never work again on a project where the stakeholders don't have at least the willingness to support practices around unit testing and continuous integration. And it has worked very well so far!

> But let me be more concrete to have a better answer for your question: what are the practices described in Clean Code that changed my way of working?

> The main one is **Unit Tests**. It is the root of my learning journey so far, because to write good Unit Tests, you have to learn about [Object Oriented](http://butunclebob.com/ArticleS.UncleBob.PrinciplesOfOod) (OO), [SOLID principles](https://en.wikipedia.org/wiki/SOLID_(object-oriented_design)), [KISS](https://en.wikipedia.org/wiki/KISS_principle) and [DRY](https://en.wikipedia.org/wiki/Don%27t_repeat_yourself). And you need a few decades just to master these principles.

> The second one is **revealing intention**. I understood that code is a story you write for a human, not for a computer. I accepted that the comments I wrote were most of the time just an excuse because of a poor implementation with bad naming.

> And basically these are the main practices I have been trying to follow day after day for the last 7 years: SOLID OO code, as simple as possible, as intuitive as possible.

What I like the most about Emilien's answer is that Clean Code principles were so important to him that he was willing to quit his job to be able to work in a way that corresponds to his values. The truth is, many developers talk about good practices such as Unit Testing and SOLID, but few actually practice them (it's like youngsters talking about sex in high school...).

At first, writing code using these best practices requires much more thought and hard work than only focusing on making our code work. But if we don't practice them, our codebase can quickly become horrible to work with, and tiny little changes can then require a lot of time and effort.

As I now work on a codebase with hundreds of thousands of lines, I see the wisdom and value of these practices. The developers I admire the most are not those who use the most clever hacks, but those who write code that is simple and clear and tested. When I see it, I understand it, and can update it if needed with confidence.

> **Emilien**: I'm thankful to have crossed your way in my journey. Thank you for having inspired me to view my work as a valued craft, and for making me want to become a software craftsman... or die trying. 
