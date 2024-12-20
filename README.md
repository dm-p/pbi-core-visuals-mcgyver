# MacGyver

> [verb] Mac·Gy·ver | mə-ˈgī-vər | MacGyvered | MacGyvering | MacGyvers

<img src="./.doc/macgyver.jpg" alt="Angus MacGyver" title="Angus MacGyver"/>

&nbsp;

> “Make or repair (an object) in an improvised or inventive way, making use of whatever items are at hand.”
> \- [Merriam-Webster](https://www.merriam-webster.com/wordplay/what-does-macgyver-mean-slang-definition)

> “[Using] the formatting options for Power BI visuals in unorthodox ways to achieve the result we want.”
> \- [Kurt Buhler](https://www.sqlbi.com/articles/creating-custom-visuals-in-power-bi-with-dax/#:~:text=we%20use%20the%20formatting%20options%20for%20Power%20BI%20visuals%20in%20unorthodox%20ways%20to%20achieve%20the%20result%20we%20want)

# Adventures in MacGyvering Power BI Core Visuals

Every now and again, I'll come up with something using core visuals that might be handy for other folks to look at, adapt and make way better than I can. I hope that you find them useful!

## 📎 Box and Whisker Plot (Clustered Bar Chart)

[ [.pbix](./box-whisker-plot-error-bars/box-whisker-plot-error-bars.pbix) ] [ [Video](https://www.youtube.com/watch?v=67ZE4qCSSw4) ]

<img src="./box-whisker-plot-error-bars/box-whisker-plot-error-bars.png" height="250"/>

A clustered bar chart, statistical measures, and error bars are used to create a layered box and whisker plot. While we could do this with a custom visual (or R/Python) using minimal effort, we can be constrained by the amount of data we can add to its dataset before Power BI will cap it, so if we have millions (or billions) of data points we want to evaluate, we can do this very quickly using DAX to compute the statistics and then using error bars to create the primitive shapes needed for a box and whisker plot and bind their attributes to these measures.
