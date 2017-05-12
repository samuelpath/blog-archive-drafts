![alt text](http://www.samuelpath.com/wp-content/uploads/2017/05/dev-mastery.png)

Last week, I continued my Clean Code series by having [Emilien Pecoul](http://www.samuelpath.com/emilien-pecoul-software-craftsman-on-clean-code/) answer the question: "What is Clean Code for you?"

Today, I have the priviledge of introducing Bill Sourour and his answer to you. I've been reading his Dev Mastery newsletter since July 2016, and I'm a better developer for it. If you don't know about it or haven't subscribed to it, you can check all his previous posts on his [Medium profile](https://medium.com/@BillSourour). And if you like what you read, you can subscribe [here](https://devmastery.com/).

Bill writes about all kinds of software-related topics, from [how to find time to become a better developer](https://medium.freecodecamp.com/finding-time-to-become-a-better-developer-eebc154881b2), to [how to conquer legacy code](https://medium.freecodecamp.com/conquer-legacy-code-f9e23a6ab758), [ethical standards for developers](https://medium.freecodecamp.com/the-code-im-still-ashamed-of-e4c021dff55e), and even [elements of JavaScript syntax and style](https://medium.freecodecamp.com/constant-confusion-why-i-still-use-javascript-function-statements-984ece0b72fd).

The breadth of topics he can address in depth thanks to his more than 20 years experience is impressive to me. Whether you agree with his conclusions or not, you can always find nourishing food for thought.

So here is what Clean Code is for him:

> Clean code is focused, deliberate, expressive and free of error.

> **Focused** in that each discrete part of it is concerned with one thing and one thing only.

> **Deliberate** in that it came to be through thoughtful, purposeful, design.

> **Expressive** in that its function, purpose, and intent are immediately obvious to all who read it.

> **Free of error** in that it works consistently as designed.

The first thing that strikes me about Bill's answer is its concision. Each word serves a specific purpose and has been carefully chosen. Another feature of his answer is how organized it is. We have an introductory statement containing 4 parts, then one sentence detailing each part. It's as if Bill applied the same Clean Code principles to the way he organizes his writing:

* Each sentence is concerned with one concept and one only.
* Each sentence has been carefully crafted and thought through.
* Each sentence can be understood by anyone upon first reading.
* Each sentence has been shipped free of typo and syntax error.

We see again great similarities between clean prose and clean code, as I already noticed following [Jan's answer](http://www.samuelpath.com/jan/). A few years ago, I read [On Writing Well: The Classic Guide to Writing Nonfiction](https://www.amazon.com/gp/product/0060891548/) by William Zinsser, which helped me become a less terrible writer. And recently, I found out that the book was on many recommending reading lists for developers, like this [recent one](https://medium.freecodecamp.com/what-to-learn-in-2017-if-youre-a-frontend-developer-b6cfef46effd). I'm convinced that good and timeless elements of style are shared between prose and code. If you know how to communicate well in English or French, you can apply the same principles to your code.

By working in a large company with more than a hundred developers, where developers communicate regularly by text (emails, wikis, etc.), I've witnessed the strong correlation between written communication and code. Some colleagues send emails without much structure and with a lot of typos and grammatical errors. Usually, these same colleagues write code that is less well crafted, and where attention to detail is not sufficiently given. As for those who take the time to communicate clearly, making sure their text is well-structured and without error, they usually apply the same care to the code they write. Sloppy writers are usually sloppy coders and vice-versa.

Now, I'd like to take each of Bill's four sentences, and share my commentaries. I hesitated to do this at first since his answer feels so *pure* to me. But if I don't give it a shot, I'll never know if I've truly understood his points.

So here we go:

> **Focused** in that each discrete part of it is concerned with one thing and one thing only.

This invokes modularity to me, the solution to one of developers' worst nightmares: spaghetti code. When a codebase is truly modular, there are many side benefits. When we have to change some behavior in our program, we don't have to apply the same change in many different parts. For instance, when we change something in our app's interface and design, we don't have to change anything on the back-end, and vice-versa.

Another benefit is that we don't have to reinvent the wheel every day. Our modular code can be exported and shared between different apps (and companies, think [NPM](https://www.npmjs.com/)). Moreover, we can only load what we need, and thus don't find ourselves loading useless code.

I'm sure we've all worked on legacy codebases where the code wasn't focused, and where it takes hours to add a button with a simple action. At least I have, and it's painful. Focused code is the answer.

> **Deliberate** in that it came to be through thoughtful, purposeful, design.

This point really challenges me. I have the bad habit of starting to code immediately, before thinking too much about the design or the architecture of my solution. And then, hours after having started, I realize that there was a more elegant way where adding a few lines of code would have solved my problem (or no code at all sometimes!). I have the same problem when writing prose. I struggle to take the time to plan. And I can thus easily fall into the trap of mindless rambling. In this regard, we need to find good balance. It's also possible to take too much time to plan and then have too little time to execute. But at least, we need to make sure to have considered the main options before racing head-first into writing code.

> **Expressive** in that its function, purpose, and intent are immediately obvious to all who read it.

There are some coding hacks that make the coder look smart but that are hard to understand for the reader. For instance in JavaScript, it's often possible to solve pretty complex problems in one line using chained Array prototype functions (such as [].map(), [].reduce() and [].filter()) and arrow functions (i.e. "=>"). But in many cases, the code is much more readable when we decompose the solution in various steps with intermediary well-named variables.

When I started as a professional developer, I was often tempted to replace code written by colleagues with some "clever hacks". I was even sometimes condescending in my heart, feeling like they should know better. Today, I realize that it was stupid, even more so when I struggle sometimes to understand code I've written myself a few months ago…

There's no point in using clever techniques if it makes the code less readable and maintainable. *Looking* smart and *being* smart are two different things!

> **Free of error** in that it works consistently as designed.

One of the only ways to make sure that our code is free of error is testing. There are many ways to test our code, and they are usually complementary:

* **Manual testing**, where we try to imagine everything a (benevolent or malicious) user could want to do, including many edge cases ("What happens if I enter an email address with the @ ?")
* **Integration testing**, where a program simulates the use by a user and makes sure everything is correctly integrated. This is a great way to make sure that future development don't break existing features.
* **Unit testing**, where we create functions to test each discrete part of our system. For instance, if a function is meant to calculate a monthly payment based on a loan's duration and rate, unit tests give various inputs with various expected outputs, and make sure the function always returns what's expected.

As a younger developer, I often felt like testing was a waste of time, and that I wasn't *really* doing the work of a developer. So during the first months in my current job, I neglected that part to have more time to code. But this was a terrible mistake! As my future code broke my previous code in many unpredictable ways (that could have been predicted using testing), I came to realize that testing my current code is an investment for the future. It has a cost today, but not doing now will cost even more in the future.

## Conclusion

Bill's concise answer has led to a quite lengthy commentary by me. Thanks for having read thus far. I hope you've found valuable insights in both. Of course, my junior developer insights don't have the same value as Bill's wise words, but I still hope you found them complementary.

> **@Bill**: Thank you so much for having granted my request. It's an honour for me to publish your answer. Thank you also for sharing the wisdom you've gained through the years with thousands of "hungry" developers like me. I hope my commentaries mainly represented what you had in mind. If not, please do not hesitate to correct or clarify.