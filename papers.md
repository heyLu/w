# Papers to read

Papers seemed intimidating for a long time, but reading and understanding them is really rewarding.  This is a collection of papers that I have found to be enjoyable/enlightening to read.

## Haskell

- [A Prettier Printer](http://homepages.inf.ed.ac.uk/wadler/papers/prettier/prettier.pdf), by Philip Wadler, designing a more efficient pretty printer than the one in std haskell.  An extended version is availlable as [wl-pprint](https://hackage.haskell.org/package/wl-pprint) on Hackage.
- [Beautiful Concurrency](http://research.microsoft.com/en-us/um/people/simonpj/papers/stm/beautiful.pdf), by Simon Peyton Jones.  Introducing (and motivating) the idea of STM.
- [Monad Transformers Step by Step](http://catamorph.de/documents/Transformers.pdf), by Martin Grabmüller.  This paper starts with a simple implementation of the lambda calculus with arithmetic, and then adds various features (proper error handling with `Either`, light debugging, state) using a stack of monad transformers.

## Language implementation

- [Pycket: a tracing JIT for a functional language](http://homes.soic.indiana.edu/samth/pycket-draft.pdf), by Sam Tobin-Hochstadt.  Describes a very fast implementation of Racket using the RPython meta-tracing framework.

## Unsorted

- [µKanren: A Minimal Functional Core for Relational Programming](http://webyrd.net/scheme-2013/papers/HemannMuKanren2013.pdf), by Jason Hemann and Daniel P. Friedman.  Describes a minimal implementation of the core primitives of miniKanren, which amount to 39 lines of Scheme.  This is a beautiful starting point for learning about the miniKanren family of languages, read William E. Byrd's thesis next if you want to learn about how the full miniKanren language is implemented.
