# Game-Programming-Patterns

# Introduction

"At first, the challenge was just getting something working. Then, it became figuring out how to write programs bigger than what would fit in my head. Instead of just reading about 'How to program in C++, I started trying to find books about how to *organize* programs.

Fast-forward several years, and a friend hand me a book: *Design Patterns: Elements of Re-usable Objects-Oriented Software*. Finally! The book I'd been looking for since I was a teenager. I read it cover to cover in one sitting. I still struggled with my own programs, but it such a relief to see other people struggled too and came up with solutions. I felt like I finally had a couple of tools to use, instead of just my bear hands.

In 2001, I landed my dream job: software engineer at Electronic Arts. I couldn't wait to get a look at some real games and see how the pros put them together. What was the architecture like for an enormous game like Madden Football? How did the different systemss interact? How did they get a single code base to run on multiple platforms?

Cracking open the source code was a humbling and suprising experience. There was brilliant code in graphics, AI, animation and visual effects. We had people who knew how to squeeze every last circle out of a CPU and put it to good use. Stuff I didn't even know was *possible*, these people did before lunch.

But the *architecture* this brilliant code hung from was often an afterthought. They were so focused on *features* that organization went overlooked. Coupling was rife between modules. New features were often bolted onto the codebase wherever they could be made to fit. To my disillutioned eyes, it looked like many programmers, if they ever cracked open *Design Petterns* at all, never got past **Singleton**.

Of course, it wasn't really that bad. I'd imagined game programmers sitting in some ivory tower covered in whiteboards, calmly discussing architectural minutiae for weeks on end. The reality was that the code I was looking at was written by people working to meet intense deadlines. They did the best they could, and, as I gradually realized, their best was often very good. The more time I spent working on game code, the more bids of brilliance I found hiding under the surface.

Unfortunately, 'hiding' was often a good description. There were gems buried in the code, but many people walked right over them. I watched coworkers struggle to reinvent good solutions when examples of exactly what they needed were nestled in the same codebase they were standing on.

That problem is what this book aims to solve. I dug up and polished the best patterns I've found in games, and presented them here so that we can spend our time inventing new things instead of *re*-inventing them.

# What's in Store

There are already dozens of game programming books out there. Why write another?

Most game programming books I've seen fall into one of two categories:

* **Domain-specific books.** These narrowly-focused books give you a deep dive on some specific  aspect of game developement. They'll teach you about 3D graphics, real-time rendering, physics simulation, artificial intelligence, or audio. These are the areas that many game programmers specialize in as there career progress.

* **Whole-engine books.** In contrast, these try to span all of the different parts of an entire game engine. They are oriented towards building a complete engine suited to some specific genre of game, usually a 3D first-person shooter.

I like both of these kinds of books, but I think they leave some gaps. Books specifiic to a domain rarely tell you how that
chunk of code interacts with the rest of the game. You may be a wizard at physics and rendering, but do you know how to tie them together gracefully?

The second category covers that, but I often find whole-engine books to be too monolithic and too genre-specific. Especially with the rise of mobile and casual gaming, we're in a period where lots of different genres of games are being created. We aren't all just cloning Quake anymore. Books that walk you through a single engine aren't helpful when *your* game doen't fit that mold.

Instead, what I'm trying to do here is more *á la carte.* Each of the chapters in this book is an independent idea that you can apply to your code. This way, you can mix and match them in a way that works best for the game *you* want to make.

> Another example of this *á la carte* style is the widely beloved [Game Programming Gems](http://www.satori.org) series.

# How it Relates to Design Patterns

Any programming book with "Patterns" in its name clearly bears a relationship to the classic *Design Patterns: Elements of Reusable Object-Oriented Software* by Erich Gamma, Richard Helm, Ralph Johnson, and John Vlissides (ominiously called the "Gang of Four").

> *Design Patterns* itself was in turn inspired by a previuos book. The idea of crafting a language of patterns to describe open-ended solutions to problems comes from [A Pattern Language](https://en.wikipedia.org/wiki), by Christopher Alexander (along with Sara Ishikawa and Murray Silverstein).

Their book
"
