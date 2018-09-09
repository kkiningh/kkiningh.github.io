---
layout: post
title: Bash Completion on OS X With Homebrew
---

Bash compleation is one of those hyperconvient features that you forget about until you have to use a system where it's not available.
Recently, I found out that many homebrew formulas come with builtin support for bash completions.
Assuming you already have [homebrew](https://brew.sh/) installed, you'll first install the bash-completion formula

```bash
$ brew install bash-completion
```

Next, add the following line to your `.bash_profile`
```bash
[ -f /usr/local/etc/bash_completion ] && . /usr/local/etc/bash_completion
```

Restart your shell, and that's it!
Now you should have bash completion support for git, [bazel](https://bazel.build/), and many other command line utilities.
