# Introducing quickstart

Hello Internet, I'd like to introduce you to `qst`. It's pronounced
"quickstart" and it's a tool that lets you get startet with projects
quickly.

When learning a new language it's often not clear how to actually run
programs in that language and what best practices are. It gets worse
when you just want to try out a tool that's written in a language you
don't yet know.

And even if you do know the language and have decided what your
favourite build system is, sometimes it's difficult to keep track of the
right commands to use.

So, why not get a little help? That's `qst`.

    $ git clone git://github.com/heyLu/expandr
    ...
    $ cd expandr
    $ qst .
    Running on http://localhost:4000

That's it. Now you've got a webserver running on <http://localhost:3000>
that is able to unshorten urls.

The project is written in Haskell, but you don't have to know that. If
you have `cabal` installed, `qst` will just run that and set everything
up.

# What else?

`qst` supports C, Clojure, Haskell, Idris, Julia, Python, Ruby,
JavaScript, Makefiles and quite few more as of now (September 2014) and
it's easy to add more. In most cases it's one line that tells `qst` how
to recognize the project and how to run it.

Some project types also support different "steps" to run, e.g. for just
building the project or running the test suite.

# What can you do with it?

Run one-file projects in any language:

    $ qst server.go
    Running on http://localhost:3000...
    ...

If you now edit `server.go` and save, `qst` will restart the server.

For one-off scripts, you can also disable restarting when your program
exits:

    $ qst -autorestart=false hello-world.c
    Hello, World!
    ...

The delay between restarts is also configurable using `-delay`:

    $ qst -delay=1m complex-thing.jl
    ...

If you just want to know the type of a project, you can do that as well:

    $ qst -detect ~/projects/uh-what-was-this-thing
    idris/default

You can also have it run just the tests or only build:

    $ qst -step=test ~/projects/rails-tutorial
    ...
    All tests passed!

# How does it work?

In most cases `qst` looks for certain files to determine the project
type, but in general you pass it a path and then it asks all it's
project types whether that path belongs to it. If a type matches, then
that project types' run step is run.

A "step" is just a tiny shell script that calls the build tool for that
project.

# What is it not?

It's not intended to replace anything, but it should help you get
started with things. It tells which commands it runs, so if you don't
like them you can have a look, read a bit and then run that.

It's also very simple, it really doesn't do much. It was mainly intended
to run things quickly and then let you do more complex things when you
need them.

# How can I get it?

Either download the [lastest version][bin-linux-64bit] (for Linux 64bit,
versions for other systems welcome!) directly, or just `go get` it:

    $ go get git://github.com/heyLu/lp/go

# Have fun!

Comments welcome! Try and see if it works for you. If it does, awesome!
If it doesn't I'd like to hear what I can do to fix that.
