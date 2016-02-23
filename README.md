# clj-async.nvim

Provides async clojure completion through [deoplete.nvim][] and
[nrepl-python-client][].

Trying to use Fireplace's omnicompletion with auto-complete is painfully
slow at times, making typing blocked. Using this module will be faster as
it does not block, it runs in it's own thread.

## Installation

Follow the install instructions for [deoplete.nvim][]. I'm not going to try
and sync them here. Then just include with your favourite plugin manager,
mine is [vim-plug][]

```vim
Plug 'SevereOverfl0w/vim-clj-async'
```

## FAQ

1. Why do you include [nrepl-python-client][] via submodule.

   I made the decision that it was more complex to have users try and
   manage a version of [nrepl-python-client][], than it was for them to
   "just" have it included. In an ideal world, I'd be able to use
   virtualenv with the Python/Neovim, but this isn't currently achievable.


[deoplete.nvim]: https://github.com/Shougo/deoplete.nvim
[nrepl-python-client]: https://github.com/cemerick/nrepl-python-client
[vim-plug]: https://github.com/junegunn/vim-plug
