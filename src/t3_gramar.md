# The Grammar of Graphics

## Common plots

Common statistical plots:
- Bar chart
- Scatter plot
- Line chart
- Box plot
- Histogram

The followings are the general rules for common plots, but theses can always be changed:

Scatter plot

- continuous varialbe vs continuous variable


Line plot

- continuous varialbe vs continuous variable

Box plot

- categorical varialbe vs continuous variable

Histogram

- continuous variable vs continuous variable

Bar chart

- categorical varialbe vs continuous variable


## What make a basic plot

<p align="center">
  <img src="images/t3/basicPlot.png" style="width:90%"/>
</p>
<p align="center">
The components for a basic plot.
</p>

Let's draw a scatterplot of **A** vs **C**.

<p align="center">
  <img src="images/t3/1.png" style="width:40%"/>
</p>
<p align="center" style="font-size: 0.775em">
  Wickham, Hadley. A Layered Grammar of Graphics.
</p>

Then Mapping A to x-position, C to y-position, and D to shape

<p align="center">
  <img src="images/t3/2.png" style="width:40%"/>
</p>
<p align="center" style="font-size: 0.775em">
  Wickham, Hadley. A Layered Grammar of Graphics.
</p>

Here we have three basic layers:
- Geometric objects
- Scales
- Coordinate system (From left to right)

<p align="center">
  <img src="images/t3/3.png" style="width:90%"/>
</p>
<p align="center" style="font-size: 0.775em">
  Three basic layers. Wickham.
</p>


#### References
[1] [Hadley Wickham, Garrett Grolemund. R For Data Science.](https://r4ds.had.co.nz/) \
[2] [Hadley Wickham, A layered grammar of graphics](https://vita.had.co.nz/papers/layered-grammar.pdf)
