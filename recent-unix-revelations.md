# recent unix revelations

talk about a grandiose title. here they are, randomly ordered.

* don't end your commit messages with dots.

    i used to do that. it's surprisingly difficult to stop doing it.

    why? because [that][c1] [seems][c2] to be [how][c3] [people][c4] do it.

    other git things i do:

    - `git add/commit -p` to split commits
    - `git merge --no-ff` to keep merges in the history

        i want to see that i implemented a feature, so a merge is a good way
        to document that.
    - `git merge --ff-only` when merging `origin/master`, e.g. so that i
        don't accidentally merge when pulling

[c1]: https://github.com/erlang/otp/wiki/Writing-good-commit-messages#dont
[c2]: http://blogs.gnome.org/danni/2011/10/25/a-guide-to-writing-git-commit-messages/
[c3]: http://tbaggery.com/2008/04/19/a-note-about-git-commit-messages.html
[c4]: https://wiki.openstack.org/wiki/GitCommitMessages#Summary_of_GIT_commit_message_structure

and maybe i'll even start [two-spacing](http://stevelosh.com/blog/2012/10/why-i-two-space/).

but wait, there are also non-unixy things:

* use [private tabs](https://addons.mozilla.org/en-US/firefox/addon/private-tab/) (for twitter, facebook and other tracking things)

    it's [not enough](https://panopticlick.eff.org/), though. tiny steps ...

(there were more, but i seem to have forgotten them.)
