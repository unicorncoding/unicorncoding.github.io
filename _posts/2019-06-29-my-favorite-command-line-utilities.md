---
layout: post
title: My Ten Favorite Command-Line Utilities
image: favorite-cli.jpg

---

Depending on tools that you use, Terminal can either make you productive or slow you down. Below you will find **ten command-line tools and utils that make me more productive**.

![Me Hacking](/images/{{page.image}})

---

1️⃣ **[tldr](//tldr.sh){: rel="nofollow" }** is a better and simpler version of `man pages`. When I forget how to use a certain unix utility, such as `chmod`, there is no better solution than typing `tldr chmod`.

2️⃣ **[fx](//github.com/antonmedv/fx){: rel="nofollow" }** is an awesome JSON processor for the command line. You can display, filter, and transform JSON without leaving the command line.

3️⃣ **[autojump](//github.com/wting/autojump){: rel="nofollow" }** is a `cd` command on steroids. `autojump` learns which directories you use and makes switching between them easier.

4️⃣ **[exa](//github.com/ogham/exa){: rel="nofollow" }** is a modern replacement for `ls`. It looks nicer, uses colours to distinguish file types and metadata, knows about symlinks, extended attributes, and Git.

5️⃣ **[bat](//github.com/sharkdp/bat){: rel="nofollow" }** is a modern replacement for `cat`. It supports syntax highlighting for a large number of programming and markup languages.

6️⃣ **[fd](//github.com/sharkdp/fd){: rel="nofollow" }** is a better and simpler version of `find`. I still can't use `find` effectively after being a Linux user for 10 years, but I have no problems understanding `fd`.

7️⃣ **[fzf](//github.com/junegunn/fzf){: rel="nofollow" }** is a fuzzy finder for a command-line. I use it together with `fd`, like this: `fd . ~/Desktop | fzf`. Forget about searching with GUI!

8️⃣ **[tmux](//github.com/tmux/tmux){: rel="nofollow" }** allows me to open and manage multiple split-views in one terminal. Spend 15 minutes [learning](//bit.ly/uni_tmux){: rel="nofollow" } `tmux` and boost your productivity 10x.

9️⃣ **[micro](//github.com/zyedidia/micro){: rel="nofollow" }** is a modern and intuitive terminal-based text editor. If you don't like Vim, Emacs and Nano, you'll like `micro`. It even has a mouse support!

🔟 **[httpie](//github.com/jakubroztocil/httpie){: rel="nofollow" }** is an awesome Http client for the command-line. It's a curl alternative with intuitive syntax, JSON support, syntax highlighting, and wget-like downloads.

⤵️ **Bonus utils for awesome developers**

🎁 **[fselect](//github.com/jhspetersson/fselect){: rel="nofollow" }** is a utility for searching files with SQL-like syntax. Isn't the following query self-describing? `fselect name from . where name = '*.mp3' and size gt 1mb`

🎁 **[peco](//github.com/peco/peco){: rel="nofollow" }** is an interactive version of `grep`. It's a great tool to filter stuff like logs, process stats, or files, because unlike grep, you can type as you think and look through the current results.

Enjoy!