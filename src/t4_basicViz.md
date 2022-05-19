# Basic Data Visualization in R

## Chart selection

A great explanation on selecting a right chart type by Dr. Andrew Abela.

but as a data scientist should not be limited by this.

<p align="center">
  <img src="images/t4/1.png" style="width:100%"/>
</p>

## Components of the plots

- Layers:
  - Dataset
  - Aesthetic mapping (color, shape, size, etc.)
  - Statistical transformation
  - Geometric object (line, bar, dots, etc.)
  - Position adjustment
- Scale (optional)
- Coordinate system
- Faceting (optional)
- Defaults

## ggplot2 full syntax

```r
ggplot(data = <DATASET>,
       mapping = aes( <MAPPINGS>) +
        layer(geom = <GEOM>,
              stat = <STAT>,
              position = <POSITION>) +
        <SCALE_FUNCTION>() +
        <COORDINATE_FUNCTION>() +
        <FACET_FUNCTION>()
```

### A typical graph template

```r
ggplot(data = <DATASET> ,
      mapping = aes(<MAPPINGS)) +
      <GEOM_FUNCTION>()
```

## Creat a plot with basic data

```r
ggplot(data=mpg)+
  geom_point(mapping = aes(x=displ>2,y=hwy))
```
<p align="center">
  <img src="images/t4/2.png" style="width:70%"/>
</p>

```r
ggplot(data=mpg[mpg$model=="a4",])+
  geom_point(mapping = aes(x=displ,y=hwy))
```
<p align="center">
  <img src="images/t4/3.png" style="width:70%"/>
</p>

## Aesthetic Mappings

The greatest value of a picture is when it forces us to notice what we never expected to see.

—John Tukey

Basic components of aesthetic mapping:
- Mapping
- Size
- Alpha
- Shape
- Color

Map the colors of your points to the class variable to reveal the class of each car:

### Aesthetic Mappings: Mapping
```r
ggplot(data = mpg) +
  geom_point(mapping = aes(x = displ, y = hwy, color = class))
```
<p align="center">
  <img src="images/t4/4.png" style="width:70%"/>
</p>

### Aesthetic Mappings: Size

Not recommend mapping an unordered variable to an ordered aesthetic:

```r
ggplot(data = mpg) +
  geom_point(mapping = aes(x = displ, y = hwy, size = class))
```
<p align="center">
  <img src="images/t4/5.png" style="width:70%"/>
</p>

### Aesthetic Mappings: Alpha

```r
ggplot(data = mpg) +
  geom_point(mapping = aes(x = displ, y = hwy, alpha = class))
```
<p align="center">
  <img src="images/t4/6.png" style="width:70%"/>
</p>

### Aesthetic Mappings: Shape
```r
ggplot(data = mpg) +
  geom_point(mapping = aes(x = displ, y = hwy, shape = class))
```
<p align="center">
  <img src="images/t4/7.png" style="width:70%"/>
</p>


> What happened to the SUVs? ggplot2 will only use six shapes at a time.
>
> By default, additional groups will go unplotted when you use this aesthetic.

R has 25 built-in shapes that are identified by numbers
<p align="center">
  <img src="images/t4/8.png" style="width:70%"/>
</p>


### Aesthetic Mappings: Color

For each aesthetic you use, the aes() to associate the name of the aesthetic with a variable to display. The aes() function gathers together each of the aesthetic mappings used by a layer and passes them to the layer’s mapping argument.
```r
ggplot(data = mpg) +
  geom_point(mapping = aes(x = displ, y = hwy), color = "blue")
```
<p align="center">
  <img src="images/t4/9.png" style="width:70%"/>
</p>


> ## Exercise
> - Which variables in mpg are categorical? Which variables are continuous? (Hint: type ?mpg to read the documentation for the dataset.) How can you see this information when you run mpg?
>
> - Map a continuous variable to color, size, and shape. How do these aesthetics behave differently for categorical versus continuous variables?


## Facets

### Facets: `facet_wrap()`


The first argument of facet_wrap() should be a formula, which you create with ~ followed by a variable name (here “formula” is the name of a data structure in R, not a synonym for “equation”).
To facet your plot by a single variable (discrete), use facet_wrap()

```r
ggplot(data = mpg) +
  geom_point(mapping = aes(x = displ, y = hwy)) +
  facet_wrap( ~ class, nrow = 2)
```





#### References
[1] [Dr. Andrew Abela, Choosing a good chart](http://extremepresentation.typepad.com/files/choosing-a-good-chart-09.pdf) \
[2] [Hadley Wickham, Garrett Grolemund. R For Data Science.](https://r4ds.had.co.nz/) \
[3] [Hadley Wickham, A layered grammar of graphics](https://vita.had.co.nz/papers/layered-grammar.pdf)\
[4] [Winston Chang, R Graphics Cookbook](https://r-graphics.org/)
