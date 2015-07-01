# sticky-feet

## Here's one way to have your footer behave "in the way that any sane person would obviously want it to". Viz:

* If the non-footer content of your page is less than one screen high, the footer should be 'glued' to the bottom of the screen 

  (Not floating above it, and not submerged below it.)
  
* If the non-footer content is more than one screen high, the footer should sit at the very bottom.

  (Not overlapping the other content.)

#### The key ingredients of this solution are:

1. Set the **html** height to 100% to ensure that the **body** is at least one screen high.

  (Why this should be necessary, and why the html element should even have a height, fuck knows.)

2. Use negative margins on **#notfooter** and **#footer** in order to pull up the page bottom.

  (Otherwise **#footer** sits off-screen.)

3. Use an invisible placeholder #pseudopod to prevent the bottom margin of the last element in **#notfooter** from shunting the **#footer** back off-screen (sigh).
