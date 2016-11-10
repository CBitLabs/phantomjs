## CBitLabs fork of PhantomJS

We've forked @trygveaa's fork for PhantomJS as it fixes a nasty webkit bug wherein the rendering engine was not respecting
the `page-break-inside: avoid` css rule on individual table elements.  Additionlly, this fork also ensures that table headers
and table footers will be repeated across page breaks.

The original author of this fork submitted a [pull request](https://github.com/ariya/phantomjs/pull/13331) against PhantomJS
master which does not appear to have been merged.  There are apparently some issues with the fix, but they don't impact our use
case so all is well.
