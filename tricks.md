# Tricks & hacks discovered over the years

## Wishes

- better email (cmdline search, good ui, sup + graphical ui?)
- better im (inline history, "scroll up to see", at least recent messages)
- persistent notifications (but not in fullscreen, except sometimes for
    urgent things, filtering)
- background task queue (with persistent logs, notification on finish)
- better shell (notebooky interface (including stored logs with output, other
    motivations currently missing), taggable/favourite commands, images/data inline)
- better rss/following (twitter is too noisy, rss is for some tumblrs,
    again: filters, "hiding", filters+github.rss=mightbeinteresting)

## All the things

* docker
    - you might want to use `docker run --rm -i -t` for experiments
    - `docker ps -a` shows all containers you have
    - `btrfs subvolume delete` helps removing containers with the btrfs backend
    - something like [flynn](http://flynn.io) would be cool (doesn't work yet, i think,
        might be overkill, maybe [dokku](https://github.com/progrium/dokku) is enough?
* duckduckgo
    - privacy
    - `!mdn ...` go directly to mozilla developer network article (also for lots of
        other things)
* emacs
    - `insert-char`: insert unicode characters, search descriptions with `<c-s>` as usual,
        see: `<m-x>insert-char<enter>left right double arrow<enter> = ⇔`
    - `package-install`
    - paredit! (basics: `<c-right>` to include the next expr, `<c-left>` to move one out)
    - `shell-mode`
    - interactivity (inline docs, variables with help)
* firefox
    - common shortcuts: `<c-l>` (focus address bar), `<c-s-t>` (get back most recently closed
        tab, works multiple times), `<c-s-e>` (tab groups, "birds eye"), `<c-s-p>` (private mode,
        where are private tabs?)
    - "search" bookmarks: `w Catamorphism` takes you to wikipedia, `t` translates, `d` duckduckgo
    - `about:config`, `about:addons`, `about:robots`
* git
    - aliases: `git l10 = git log -n10`, `git st = git status --short`, `git ba = git branch --all`
    - server/url aliases: `git clone hub:heyLu/muq -> git clone git://git.github.com/heyLu/muq`
    - incremental commands: `-p` (for add, checkout, commit, stash save and possible more)
    - `git pull --ff-only` (`git pull --rebase` if it complains)
    - `git merge -ff-only` (i like merge commits for everything)
    - `git diff --word-diff` when you can't see the change
    - `git diff --staged`, to see changes about to be committed
* github: `@mentions`, `:emoji:` :sparkles:, issue links `heyLu/w#1` (heyLu/issue#1)
* makefiles
    - minimal, tracks "dependencies", general rules
    - most recent/common rule on top (`make` will execute it)
    - `make <program>` (compiles it)
    - `make run`, `make run-server`
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
    - `cd = cd ~ = cd $HOME`
    - `xargs`
    - `fg`, `bg` (zsh completion helps here)
* quodlibet: for music, makes retagging/renaming easy, fancy search which i don't use much
* unix
    - the silver searcher (`ag`, like `ack`, which is like `grep`; but faster)
    - directories sorted by size: `du -h --max-depth=3 | sort -h`
    - use real regexps: `-E` (with `grep`, `sed`)
    - `pkill -f ...`, `pgrep -fl ...`
    - `watch`
* web dev
    - search for `mdn ...` (mozilla developer network)
    - http://devdocs.io is quite good (and fast)
    - [Dash](http://kapeli.com/dash) is cool, but for mac, [zeal](https://github.com/jkozera/zeal)
        works on linux, but is buggy
    - http://caniuse.com
    - in firefox: `<c-s-i>` (inspector), `<c-s-m>` (responsive design mode)
    - tools/libraries:
        * [d3](https://github.com/mbostock/d3)
        * [react](http://facebook.github.io/react), in particular when used with
            [om](https://github.com/swannodette/om)
* zsh
    - why zsh?
        * completion from directories (`~/p/has/gre-go<tab> -> ~/projects/haskell/great-good`)
            to options for commands (`git <tab>` lists subcommands, `ls -<tab>` lists options)
        * custom prompt was easier for me
    - ??? :)
