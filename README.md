pdoc
====

pdoc is (or rather, is planned to be) a PHP documentation generator and viewer. 

Currently, pdoc is a basic replacement for `pman`, the offline CLI documentation viewer provided by the PHP project. `pman` is a small wrapper script for builtin `man` command along with the function and class documentation from the PHP website in manpage format. It also appears to have not been updated since the PHP 5.6 days.

Installation
------------

The easiest way to install pdoc is with [Composer](https://getcomposer.org):

    composer global require pdoc/pdoc

Then make sure `$COMPOSER_BIN_DIR` is in your `$PATH`.

Usage
-----

Usage is easy:

    pdoc <class/function name>

For example:

    pdoc DateTime

More features are planned, so stay tuned.

Yet Another PHP Documentation Generator? Really?
-------------------------------------------------------

Yes, really.

Does the world need this? Probably not. There are a number of mature, feature-rich documentation generators available for PHP, and you're certainly better off using one of them (at least for now!). In no particular order, here's a few you might want to look at:

- [phpDocumentor](http://www.phpdoc.org/)
- [ApiGen](https://github.com/apigen/apigen)
- [Sami](https://github.com/FriendsOfPHP/Sami)
- [phpDox](http://phpdox.de)

**So why do this?**

**The TL;DR version:** because I can.

**The slightly longer version:** I've used all of the listed documentation viewers on various projects over time, and none of them really worked particularly great in my opinion. So I took a peek under the hood to see how they worked, and started wondering if I could do any better. Eventually I got to the point where I decided to give it a try.
