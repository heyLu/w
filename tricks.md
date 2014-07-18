# Tricks & hacks discovered over the years

## Wishes

- better email (cmdline search, good ui, sup + graphical ui?)
- better im (inline history, "scroll up to see", at least recent messages)
- persistent notifications (but not in fullscreen, except sometimes for
    urgent things, filtering)
- background task queue (with persistent logs, notification on finish)
- better shell (notebooky interface (including stored logs with output, other
    motivations currently missing), taggable/favourite commands, images/data inline)

## All the things

* docker
    - you might want to use `docker run --rm -i -t` for experiments
* duckduckgo
    - privacy
    - `!mdn ...` go directly to mozilla developer network article (also for lots of
        other things)
* emacs
    - `insert-char`: insert unicode characters, search descriptions with `<c-s>` as usual,
        see: `<m-x>insert-char<enter>left right double arrow<enter> = ⇔`
    - `package-install`
    - paredit! (basics: `<c-right>` to include the next expr, `<c-left>` to move one out)
* firefox
    - common shortcuts: `<c-l>` (focus address bar), `<c-s-t>` (get back most recently closed
        tab, works multiple times), `<c-s-e>` (tab groups, "birds eye"), `<c-s-p>` (private mode,
        where are private tabs?)
    - "search" bookmarks: `w Catamorphism` takes you to wikipedia, `t` translates, `d` duckduckgo
* git
    - aliases: `git l10`, `git st`, `git ba`
    - server/url aliases: `git clone hub:heyLu/muq -> git clone git://git.github.com/heyLu/muq`
    - incremental commands: `-p` (for add, checkout, commit, stash save and possible more)
    - `git pull --ff-only` (`git pull --rebase` if it complains)
    - `git merge -ff-only` (i like merge commits for everything)
* random
    - http://explainshell.com
    - offlineimap, mutt (`-Z`), geary, intellij idea, vim, msmtp
    - [Pinboard](https://pinboard.in) for bookmarks, including the firefox extension
        (the author is awesome, i paid for it, it doesn't do much, it *makes
         me think more*!)
* shell
    - incremental backwards history search (`<C-r>clone -> git clone git://...`)
    - readline bindings (`<c-a>` start of line, `<c-e>` end of line, `<c-k>` kill to end of line,
        `<m-b>`, `<m-f>`)
* unix
    - the silver searcher (`ag`, like `ack`, which is like `grep`; but faster)
    - directories sorted by size: `du -h --max-depth=3 | sort -h`
    - use real regexps: `-E` (with `grep`, `sed`)
* web dev
    - search for `mdn ...` (mozilla developer network)
    - http://devdocs.io is quite good (and fast)
    - [Dash](http://kapeli.com/dash) is cool, but for mac, [zeal](https://github.com/jkozera/zeal)
        works on linux, but is buggy
    - http://caniuse.com
    - in firefox: `<c-s-m>` (responsive design mode)
* zsh
    - why zsh?
        * completion from directories (`~/p/has/gre-go<tab> -> ~/projects/haskell/great-good`)
            to options for commands (`git <tab>` lists subcommands, `ls -<tab>` lists options)
        * custom prompt was easier for me
    - ??? :)
