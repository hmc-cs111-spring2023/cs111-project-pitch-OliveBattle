# Project proposal

## The user and a language

This section describes who the project would serve and why a language might be a
good way to meet their needs.

	This DSL is aimed for those who want to create sheet music and chord progressions or melodies quickly, and who don't have that much experience with programming.

### What's the need?

_What need is met by your idea? Who are you helping? What is that person's
experience like now? What would their experience be like if you could help
them?_

	I'm aiming to create a program that would let them quickly prototype things, without having to go through all the hurdles of designing things in a full music production application.

### Why a language?

_Why is a DSL appropriate for your user(s)? How does it address the need?_

	A language lets you design these fast, in a way that's easy to edit, and in a way that you can easily export to different forms using existing libraries. This helps to make it a quick way to prototype melodies and such, rather than having to use a graphical representation of notes that may be slower. (built in repetition and ways to vary it, especially, should be an good way to specificaully work towards this need.)

### Why you?

_What excites you about this idea? How did you come up with it?_

	I came up with it as a good project that allows me to design something novel, with unique skills added. It also lets me design a project about a domain I already have a little bit of experience in.

### Domain

_Describe the project's domain in five words._

	Producing sheet music or melodies

### Interface (syntax)

_How might the user interact with the language? What does programming look
like? Why is this the right way to interact with the problem domain?_

	A user interacts with this language by writing a new song in plaintext. The user would define a number of chords and melodies as a collection of notes, then would put together these chords and melodies in increasinly complicated ways to eventually lead to a final song. This lets you define a structure and then use it repeatedly, which should make it quicker to edit structures used across the program.

### Operation (semantics)

_What might happen when a program runs? How does a program interact with the
user? What kinds of errors might occur, and how might they be communicated to
the user?_

	When the program runs, it'll parse the plaintext file into labels for defined sets of notes, and output commands. When it comes across an output command (like creating a sheet music image, or sound file), It'll add all the given notes into that output file-whenever it comes across a label, it'll replace that with the notes it's comprised of, then modified by things like repeating some melody.

### Expressiveness

_What should be easy to do in this language? What should be possible, but
difficult? What should be impossible or very difficult?_

	It should be easily possible to define a melody or chord quickly, and it should also be possible to put those together in order to make a full 'song.' Ideally, it should be easy to take a set of notes and modify it in some way- shift it's key or repeat it or cut it short. It should be possible, but difficult, to design an entire song that's not built up out of smaller parts.

### Related work

_Are there any other DSLs in this domain? If not, describe how you know there
aren't and conjecture why not. If so, describe them and provide links. How well
do they address the need? Are there any particularly admirable qualities of the
language? Are there parts of the language you think could be improved?_

	One DSL that already exists for this domain is [Alda](https://alda.io/). This language is designed for taking text representing music notes and being able to quickly turn those into audio, and it addresses this need relatively well. One of the very admirable parts of it is just how much variation it allows you to do for the music.

## The Project

This section examines whether the idea makes for a good CS 111 project.

### Suitability

_If someone were to work on this project, what percentage of their time would be
spent directly engaging in the **language** aspects of this project (e.g.,
making language design decisions), as opposed to "systems" aspects of the
project (e.g., implementing a complicated semantics that doesn't require a lot
of language design)?_

	External DSLs are generally all going to be heavy on implementing semantics, but I still think the language has a lot of design decisions that will end up making it worthwhile as a project.

### Scope

_How big an idea is this? How ambitious is this project?_

	It's a relatively large project. One big issue with it is that it's easy to slowly add on more and more features. The looser I am with the limits around what to design, the more work the project could grow into, so it's important to go in with a specific plan for this project.

### Benefits and drawbacks

_Why might this be a good idea for a project? Why might this not be a good idea
project?_

	The main benefit for this project is a lot of opportunity to make design decisions in the language. Its status as an external DSL and the requirements to syntax with other libraries, though, end up making it more complex and probably nto the perfect project.
