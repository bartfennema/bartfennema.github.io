Welcome to my git-based (not necessarily GitHub-based!), decentralization-friendly,
liberated, and integrity-protected blog and website!

About Me
=========




About this Website/Blog/Repo
=============================

This blog is based on Joanna Rootkovska's wonderful blog.
(will write more to address licensing info)


Content of this repo
---------------------

* All my blog posts (in the [_posts/](/blog/) directory)
* [Contact info](/contact/) and my [GPG keys](/keys/)
* Other info about myself and my maybe about my work

Distribution and hosting
-------------------------

This blog/website is distributed as a git-repo, and is primarily hosted on my
GitHub account. You should be able to clone it using the following command:

    git clone https://github.com/bartfennema/bartfennema.github.io

although you'd better check out [this site](https://github.com/rootkovska/rootkovska.github.io)

You can also view the sources at GitHub online
[here](https://github.com/bartfennema/bartfennema.github.io).

This blog is also available for traditional Web-based viewing via the following
URL (which is likely how you're reading it now):

* http://rimram.mieterseboel.nl/

That URL might change in the future, as well as alternative ones might be added.

One can get notifications about new posts/updates via:

* The blog's [RSS feed](/feed.xml) (not sure)
* [My GitHub Account] (https://github.com/bartfennema/)


Integrity protection
---------------------

This blog/repo is integrity protected using [git
tags](https://www.kernel.org/pub/software/scm/git/docs/git-tag.html) digitally
signed with [my blog-signing key](/keys/). In order to verify the
authenticity of all or any of the posts, you can use the following command:

    $ git describe --exact-match HEAD
    <some tag>
    $ git tag -v <some tag>

(In)dependency on GitHub
-------------------------

While this repo is hosted on GitHub, and some GitHub-specific features are
exploited in order to make this more available to a wider audience,
specifically GitHub's support for [Static Web
Hosting](https://pages.github.com/), it should be stressed that neither
availability nor integrity of this blog requires one to use or trust GitHub.
If, for some reason, GitHub, or an ISP, or whoever in between, decided to
block, falsify, or censor this blog, there are dozens of alternative ways of
how this repo (blog) could be delivered, e.g. via Tor or other transports, and
thanks to using git signed tags, its integrity could be always verified. All
the documents contained in this repo (apart from the old Blogger posts which
have been converted automatically) have been created with an assumption to be
easily readable using just a standard text editor or viewer.

Patches or pull requests welcome!
----------------------------------

If you find spelling, grammar or other errors in my blog posts, and feel like
correcting them, please send me a patch like you would do for any other
git-based software project. Thanks! (I might not know what to do with it yet, 'cause i'm a git n00b, but I don't mind)

License/Copyrights
-------------------

This Blog and Website by Joanna Rutkowska is licensed under a [Creative Commons
Attribution-NonCommercial-ShareAlike 4.0 International
License](http://creativecommons.org/licenses/by-nc-sa/4.0/).

