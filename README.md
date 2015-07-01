# sticky-feet

# Here's one way to have your footer behave "in the way that any sane person would obviously want it to". Viz:

* If the non-footer content of your page is **less than one screen** high, the footer should be 'glued' to the bottom of the screen - not floating above it, and not submerged below it
* If the non-footer content is **more than one screen** high, the footer should sit at the very bottom, not overlapping the other content.

The key ingredients of my solution are:

1. Set the _html_ height to 100% to ensure that the _body_ is at least one screen high (why this should be necessary, and why the html element should even have a height, fuck knows.)
2. Use negative margins on _#notfooter_ and _#footer_ in order to pull up the page bottom. (Otherwise _#footer sits off-screen.)
3. Use a placeholder #pseudopod to _prevent the bottom margins of elements #notfooter from shunting the #footer back off-screen_ (sigh).

Fuck my life.
