Since starting this blog, I've had the priviledge of interviewing a few software developers I respect, with one simple question: _What is Clean Code for you?_

Since I've put the series on hold for a few months, here are a refresher of the articles so far:

- [Intro to the series and answers from giants from the book "Clean Code"](http://www.samuelpath.com/what-is-clean-code/)
- [Jan, Senior Software Engineer at Mozilla](http://www.samuelpath.com/jan/)
- [Ben, Compiler Engineer at Mozilla](http://www.samuelpath.com/ben/)
- [Emilien Pecoul, Software Craftsman](http://www.samuelpath.com/emilien-pecoul-software-craftsman-on-clean-code/)
- [Bill Sourour from Dev Mastery](http://www.samuelpath.com/bill-sourour-from-dev-mastery-on-clean-code/)

In June from last year, I sent an email to Cory House, a pretty famous and in-demand developer, so I didn't really expect a response. I've tried in the past to do the same with other notorious developers, who never came back to me (and that's fine, they must receive hundreds of emails per week from strangers with all kinds of requests).

So I was delighted to see him provide an answer, in only one sentence. But before sharing it, here are a few words on Cory, from his [Pluralsight profile](https://www.pluralsight.com/authors/cory-house) where he's a popular teacher:

> Cory is an independent consultant with over 15 years of experience in software development. He is the principal consultant at [reactjsconsulting.com](http://reactjsconsulting.com/) and a [Microsoft MVP](https://mvp.microsoft.com/). As a software architect at Cox Automotive, Cory creates web applications for the automotive industry using C#, .NET, Node, and JavaScript. Cory has trained over 10,000 software developers at conferences and businesses worldwide on clean coding practices, front-end development, testing, and software architecture. He speaks regularly at conferences like NDC, Fluent, and Codemash. Cory lives in Kansas City where he blogs at [bitnative.com](https://www.bitnative.com/) and is active on Twitter as [@housecor](https://twitter.com/housecor).

As for my relationship with Cory, I've been following him for almost two years on [Twitter](https://twitter.com/housecor) and [Medium](https://medium.com/@housecor) and have been regularly encouraged to grow both as a developer and a human being as a result. I've also listened to a few interviews from him on [various podcasts](https://www.google.com/search?q=podcast+cory+house) and followed one of his courses on [Becoming an Outlier](https://www.pluralsight.com/courses/career-reboot-for-developer-mind).

If you haven't heard from him yet, I'd encourage you to take a few minutes to check some of his resources available online and follow him on Twitter. This won't be wasted time.

Okay, enough for the intro, here is his answer to the question: _What is Clean Code for you?_

> Clean code clearly expresses the programmer's intent in bite-sized pieces that can be reasoned about in isolation.

That's it. That's indeed an answer that clearly expresses Cory's intent in a bite-sized piece that can be reasoned about in isolation, right? 😋

So let me walk you through the answer.

# Clean code is clear…

Actually, I wonder why we're using the adjective "Clean" when talking about code. To me, "Clean Code" is all about _clarity_. We could rename the movement and call it "Clear Code" instead of "Clean Code".

When I need to dive in a new codebase, the best gift the original writers could have left me is clarity. It's again the same as with writing prose.

# It expresses the programmer's intent…

And what is clarity but simply transparence about the author's intent?

When trying to understand code I didn't write, the most common and frustrating questions that come to me are: _But why? Why did you write this that way? What did you mean? What were you thinking?_

Clean code doesn't leave you wondering. It uses the chosen language's idioms and best practices to translate intent into code.

All the variables and functions are carefully named to reflect what they're referring to. Good naming is key. Just the right combination of words with the right nuance so that the meaning becomes unmistakable. It simply cannot mean something else in its context. No ambiguity can be tolerated.

The cleaner the code, the less questions a reader needs to ask himself to understand it. You feel like you are in the author's mind.

Yet again, we see that writing good code is all about being a good communicator. We write code for humans before writing it for machines. We write to be read and understood.

It's almost impossible to be a clean coder and yet not be able to communicate clearly with other human beings. The two go hand in hand. The myth of the lone coder in a cave with long hair needs to die. These folks are most likely not clean coders. They may get things done for sure, but having to dive into their codebase would be a nightmare for most of us.

# …in bite-sized pieces that can be reasoned about in isolation

Another key ingredient to clean code.

I still remember vividly the time I had to dive into a huge codebase where some files had more than 10,000 lines and where some functions were hundreds of lines long.

To understand the logic, I had to start at the top, put my headphones on, and struggle through a jungle of cascading _for_ loops and _if_ statements.

In his book Clean Code, Bob Martin says the following:

> The first rule of functions is that they should be small. The second rule of functions is that they should be smaller than that. Functions should not be 100 lines long. Functions should hardly ever be 20 lines long.

When you look at some of the most successful open source projects on Github, you'll be hard pressed to find functions longer than 20 lines. Here's an [example](https://github.com/Microsoft/vscode/blob/master/src/main.js) from the source code of [Visual Studio Code](https://code.visualstudio.com/), the editor I'm using to write this article. Even if you are not familiar with this codebase, you can quickly make sense of the logic since the functions are clearly named and short.

