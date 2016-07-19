# lts-convenience
A collection of scripts to automate tracking, patching, and building
one's prefered upstream LTS branch of Linux.

  * autopatch: checks for the latest sublevel update for your
    linux-$VERSION.$PATCHLEVEL, and downloads and applies all patches
	needed to bring your tree up to this level.  In the future it will
	also support tracking the realtime patch-set, the -ck patch-set,
	or the BFQ patch set.
  * build-kernel: a wrapper around Debian's make-kpkg that chooses a
    more sensible default EXTRAVERSION, enables appropriate
	concurrency, and then compiles using a specific GCC version.

I've been using these for years...at some point I plan deeper
integration into the existing Debian tools, and at some point
I might even stop using them altogether in preference for the
official Debian packaging tools.
