# Debug log

Your notes. One entry per bug you fixed, using the template below.

This file is read as carefully as your code. A correct fix you cannot
explain counts for little; a bug you could not fix but investigated
honestly still counts for something.

Delete the example before you submit.




## CC-01-Search suggestions appear behind page elements
**Reproduced:** Search suggestions appeared behind other page elements.

**Cause:** .search-wrap had z-index: 1.

**Fix:** Increased z-index to 50.

**Checked:** Suggestions appeared in front and could be selected.

**Time:** [15 mins wont be lying was searching foer smthng else]


## CC-02 — "Dish names and prices are hard to read in dark mode"

**Reproduced:** When dark mode was enabled, dish names and prices were difficult to read because the text colour did not adapt to the dark theme.

**Cause:** The .dish-body CSS rule used a fixed text colour instead of following the theme's text colour variable.

**Fix:**I first changed the text colour to white, which improved visibility in dark mode but made the text difficult to read in light mode. I then removed the fixed colour and used the existing --ink CSS variable so the text follows the active theme.

**Checked:** [ested both light and dark modes. Dish names and prices are readable in both modes.]

**Time:** [setting up took 10 mins this fix took 8 mins.]

## CC-06-I ordered more than they had” fix kar rahe the.
**Reproduced:** When an order quantity exceeded the available stock, the order could be accepted and stock could become negative.

**Cause:** The `reserveStock()` function deducted the requested quantity without checking whether enough stock was available.

**Fix:** I added a stock availability check before deducting the quantity. If stock is insufficient, the function now returns an error and rejects the order.

**Checked:** Tested with 2 items in stock and an order quantity of 5. The order was rejected, and the original stock remained 2.

**Time:** [30 mins with ai i took help of ai cusss i want able yo find my mistakes]



## Could not fix

For anything you investigated but did not solve. Say what you tried and
where you got to. This is worth marks — leaving it blank when you got
stuck is not.

### CC-03 — "<the complaint>"

**What I tried:**Checked the mobile view and inspected the layout and scrollbar behaviour. Tried to identify the element causing the overflow, but the issue remained.

**Where I got to:**The mobile menu still overflows on smaller screens. I could not identify the exact cause or complete the fix.

**What I would try next:**Inspect the mobile menu's CSS using browser DevTools, identify the element extending beyond the viewport, and adjust its width, positioning, or overflow behaviour. Then retest at different mobile screen sizes.



## Extra credit

Anything not on the bug log: a problem you found yourself, a test you
wrote, or a fix you are unsure about. Same format, plus one line on how
you noticed it.
