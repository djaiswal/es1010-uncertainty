# es1010-uncertainty

Four interactive web pages on quantifying uncertainty in tree biomass, for Ecology & Environment 2026, IIT Palakkad. They prepare you for the class project: estimating the biomass of the trees you measured in the Miyawaki plot, and saying how sure you are of the number.

Site: https://djaiswal.github.io/es1010-uncertainty/

The pages are written in plain English. Every short form (SD, CV, AGB, …) is spelled out where it first appears, and each page starts with a "Words used on this page" box.

## Read the pages in this order

Each page builds on the one before it. Do not skip ahead.

1. **`1_dice_bootstrap.html` — From Dice to a Tree.** What "probability 1/6" really means. How to guess a hidden die from its rolls. Why the average of many rolls has less spread than one roll. The same ideas applied to 250 readings of one tree. Then two tools: the bootstrap (when you have many readings) and Monte Carlo (when you have only one reading and must assume the error).
2. **`2_equation_born.html` — How an Equation Is Born.** The tree-weight equation AGB = 0.0673 × (ρ × D² × H)^0.976, read one piece at a time and seen as a picture on log axes. How a and b are found from harvested trees. Its two kinds of doubt: Doubt 1, a and b are not known exactly (small, shared by all trees); Doubt 2, a real tree is not on the line (large, different for every tree).
3. **`3_one_tree_montecarlo.html` — Monte Carlo, One Tree.** Five dice, one for each uncertain input, rolled 20,000 times to build a pile of possible weights for one tree. How to read the pile (median, mean, SD, CV, 95 % interval), which die matters most, and how to write the result.
4. **`4_from_trees_to_plot.html` — From 25 Trees to a Plot.** A three-tree example worked by hand, then 25 measured trees added up. Why the total is known to about ± 12 % when each tree is only ± 40 %, why shared errors do not cancel, and what a per-hectare number means.

## How to work through a page

- Read the "Words used on this page" box first.
- Press **Step** once or twice and watch what one step does. Then press **Play** at slow speed. Press **Fast-forward** only once you understand one step.
- Change the inputs and watch what happens. Nothing you do can break the page; **Reset** brings it back.
- The pages run entirely in your browser. Nothing is uploaded. The numbers on them are examples.

## For the project

The project asks you to turn your field measurements into a biomass number with an honest uncertainty. The pages give you everything you need:

1. **Your data.** For each tree: species, diameter D at 1.3 m (cm), height H (m). Take the wood density ρ (g/cm³) for each species from a published table. Page 2, Panel A shows how these go into the equation.
2. **One tree.** Follow page 3. Decide the size of each die for your own readings (page 1, Panel D shows how a group of readings gives a CV). Report the median and the 95 % interval, not a single number, and say which die matters most.
3. **The whole plot.** Follow page 4. Add the trees up round by round, as in the three-tree example. Remember which errors are shared (the equation for all trees, the density value for all trees of one species) and which are independent (your readings of each tree, the scatter of each tree).
4. **Write it up** the way page 3, Panel E shows: the middle value, the 95 % interval, how many draws, and the biggest source of error. If you convert to per hectare, repeat the warning from page 4, Panel D: the interval covers measurement and equation error only, not the question of which few square metres you happened to measure.

## Files

- `index.html` — landing page linking the four pages
- `1_dice_bootstrap.html`, `2_equation_born.html`, `3_one_tree_montecarlo.html`, `4_from_trees_to_plot.html` — the four pages, in reading order
