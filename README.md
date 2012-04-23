# NOTICE: DO NOT USE THIS REPOSITORY.  THE UPSTREAM MAINTAINERS NOW PROVIDE THIS PLUGIN.  THIS PROJECT IS DEPRECATED.

# [Upstream (Github)](https://github.com/vim-scripts/paredit.vim)
# [Upstream (Bitbucket)](https://bitbucket.org/kovisoft/paredit)

## Overview

This is a version of [slimv][1] for Vim with everything removed except
the excellent paredit mode.  This allows it to be used with VimClojure,
which I personally find more useful than slimv.

  [1]: https://github.com/ibdknox/cljs-watch

## Changes Specific to This Fork

I found it difficult to use paredit mode with paren-balancing enabled for
the "change" action (e.g. commands starting with `c`).  The change action
would succeed, but subsequently repeating it with the `.` command would fail.
Thus, I disabled paren-balancing for change actions.

If you want to re-enable it, search the paredit.vim source for `FIXME: PareditChange`,
and you'll find all the code that I've disabled.  Uncomment it to taste.
