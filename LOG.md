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




## Could not fix

For anything you investigated but did not solve. Say what you tried and
where you got to. This is worth marks — leaving it blank when you got
stuck is not.

### CC-0X — "<the complaint>"

**What I tried:**

**Where I got to:**

**What I would try next:**



## Extra credit

Anything not on the bug log: a problem you found yourself, a test you
wrote, or a fix you are unsure about. Same format, plus one line on how
you noticed it.
