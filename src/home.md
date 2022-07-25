# Introduction

<!-- <p align="center">
  <img src="images/home/Minard.png" style="width:100%"/>
</p>
<p align="center" style="font-size: 0.775em">
  Creator: Charles Joseph Minard
</p> -->

**Instructor/Author:** Zhenyuan Lu

**Version:** 0.1.0

**This is the course notes** for IE6600 Computation and Visualization course, which has covered the following semesters:


<img src='https://raw.githubusercontent.com/tidyverse/tidyverse/main/man/figures/logo.png' align="right" height="55.5"/>
<img src='https://raw.githubusercontent.com/rstudio/shiny/main/man/figures/logo.png' align="right" height="55.5"/>
<img src='https://raw.githubusercontent.com/rstudio/rmarkdown/main/man/figures/logo.png' align="right" height="55.5"/>




- [Summer 22](https://zhenyuanlu.com/ie6600-bos-su22/), [Spring 22](https://zhenyuanlu.com/ie6600-sea-sp22/), [Fall 21](https://zhenyuanlu.com/ie6600-bos-fa21/), [Summer 21](https://zhenyuanlu.com/ie6600-bos-sm21/), [Spring 21](https://zhenyuanlu.com/ie6600-sea-sp21/), [Fall 20](https://zhenyuanlu.com/ie6600-bos-fa20/), Spring 20, Spring 19


## Description

IE6600 covers basic of the R, and R Shiny for data preprocessing, and visualization. It introduces students to static and interactive visualization, dashboard, and platform that reveal information, patterns, interactions, and comparisons by paying attention to details such as color encoding, a shape selection, spatial layout, and annotation. Based on these fundamentals of analytical and creative thinking, the course then focuses on data visualization techniques and the use of the most current popular software tools that support data exploration, analytics-based storytelling and knowledge discovery, and decision-making in engineering, healthcare operations, manufacturing, and related applications.



## Textbooks

**Most of the course materials are borrowed from the following books/resources.**

- [R For Data Science](https://r4ds.had.co.nz/) (**R4DS**), Wickham, Hadley, and Garrett Grolemund
- [R For Everyone](https://onesearch.library.northeastern.edu/permalink/f/365rt0/NEU_ALMA51284955070001401) (**R4E**), Lander, Jared P.
- [R Markdown](https://bookdown.org/yihui/rmarkdown/) (**RMD**), Xie, Yihui, et al.
- [Shiny tutorial](https://shiny.rstudio.com/tutorial/), R Shiny

### R-related Materials

- [R Graphics Cookbook](https://r-graphics.org/) (**RGC**), Chang, Winston.
- [Advanced R](http://adv-r.had.co.nz/) (**ADR**), Wickham, Hadley.
- [R Packages](http://r-pkgs.had.co.nz/) (**RPK**), Wickham, Hadley.
- [Text Mining with R](https://www.tidytextmining.com/) (**TM**), Silge, Julia, and David Robinson.

***

## Lectures


<table>
<!-- =============================== HEADER ================================ -->
  <thead>
    <tr>
      <th align="left">Topic</th>
      <th align="left">Slides</th>
      <th align="left">Textbook/Materials</th>
    </tr>
  </thead>
  <tbody>
<!-- =============================== Topic 1 ================================ -->
    <tr>
      <td rowspan="2"><a href="t1_basicR.md">Basic of R</a></td>
      <td rowspan="1">
        <a href="https://zhenyuanlu.com/slides/t02BasicR.pdf">📑</a>
      </td>
      <td rowspan="1">
        <b>R4E</b> "Basics of R"
      </td>
    </tr>
    <tr>
      <td><a href="https://zhenyuanlu.com/slides/t02IntroR.pdf">📑</a></td>
      <td><b>R4E</b> "Advanced Data Structure"</td>
    </tr>
<!-- =============================== Topic 2 ================================ -->
    <tr>
      <td rowspan="3"><a href="t2_grammar.md">R functions and the grammar of visualization</a></td>
      <td rowspan="3"><a href="https://zhenyuanlu.com/slides/t03RGrammar.pdf">📑</a></td>
      <td rowspan="1">
        <b>R4DS</b> <a href="https://r4ds.had.co.nz/workflow-basics.html">Workflow</a>
      </td>
    </tr>
    <tr>
      <td>
        <b>Wickham</b> <a href="https://vita.had.co.nz/papers/layered-grammar.pdf">A layered grammar of graphics</a>
      </td>
    </tr>
    <tr>
      <td>
        (optional) <b>R4E</b> "Writing R functions"
      </td>
    </tr>
<!-- =============================== Topic 3 ================================ -->
    <tr>
      <td rowspan="2"><a href="t3_basicViz.md">Basic data visualization in R</a></td>
      <td rowspan="2"><a href="https://zhenyuanlu.com/slides/t05DataViz.pdf">📑</a></td>
      <td rowspan="1">
        <b>R4DS</b> <a href="https://r4ds.had.co.nz/workflow-basics.html">Data Visualization with ggplot2</a>
      </td>
    </tr>
    <tr>
      <td>
        (optional) <b>RGC</b>"Quickly Exploring Data"
      </td>
    </tr>
<!-- =============================== Topic 4 ================================ -->
    <tr>
      <td><a href="t4_transData.md">	Data transformation with dplyr</a></td>
      <td rowspan="1"><a href="https://zhenyuanlu.com/slides/t06DataTrans.pdf"> 📑</a></td>
      <td rowspan="1">
        <b>R4DS</b> <a href="https://r4ds.had.co.nz/transform.html">Data Transformation with dplyr</a>
      </td>
    </tr>
<!-- =============================== Topic 5 ================================ -->
    <tr>
      <td rowspan="3"><a href="t5_dataWrangling_trt.md">Data wrangling with tibbles, readr and tidyr</a></td>
      <td rowspan="3"><a href="https://zhenyuanlu.com/slides/t07DataWrg_trt.pdf"> 📑</a></td>
      <td rowspan="1">
        <b>R4DS</b> <a href="https://r4ds.had.co.nz/tibbles.html">Tibbles with tibble</a>
      </td>
    </tr>
    <tr>
      <td>
        <b>R4DS</b> <a href="https://r4ds.had.co.nz/data-import.html">Data Import with readr</a>
      </td>
    </tr>
    <tr>
      <td>
        <b>R4DS</b> <a href="https://r4ds.had.co.nz/tidy-data.html">Tidy Data with tidyr</a>
      </td>
    </tr>
<!-- =============================== Topic 6 ================================ -->
    <tr>
      <td rowspan="1"><a href="t6_dataWrangling_sf.md">(optional) Data wrangling with stringr, forcats</a></td>
      <td rowspan="1"><a href="https://zhenyuanlu.com/slides/t07DataWrg_sf.pdf"> 📑</a></td>
      <td rowspan="1">
        (optional) <b>R4DS</b>"Strings with stringr", "Factors with forcats"
      </td>
    </tr>
<!-- =============================== Topic 7 ================================ -->
    <tr>
      <td><a href="t7_relational.md">Visualizing Relational Data</a></td>
      <td rowspan="1"><a href="https://zhenyuanlu.com/slides/t08RelationalData.pdf"> 📑</a></td>
      <td rowspan="1">
        <b>R4DS</b> <a href="https://r4ds.had.co.nz/relational-data.html">Relational Data with dplyr</a>
      </td>
    </tr>
<!-- =============================== Topic 8 ================================ -->
    <tr>
      <td rowspan="2"><a href="t8_shiny.md">Introduction to Shiny</a></td>
      <td rowspan="1"><a href="https://zhenyuanlu.com/slides/t09IntroToShiny.pdf">📑</td>
      <td rowspan="2">
        <b>R Shiny</b> <a href="https://shiny.rstudio.com/tutorial/">Shiny tutorial</a>
      </td>
    </tr>
    <tr>
      <td><a href="https://zhenyuanlu.com/slides/t10ShinyApp.pdf">📑</a></td>
    </tr>
<!-- =============================== Topic 9 ================================ -->
    <tr>
      <td><a href="t9_eda.md">Exploratory data analysis and more data visualization</a></td>
      <td rowspan="1"><a href="https://zhenyuanlu.com/slides/t11AppDataViz.pdf">📑</td>
      <td rowspan="1">
        <b>R4DS </b> <a href="https://r4ds.had.co.nz/exploratory-data-analysis.html">Exploratory Data Analysis</a>
      </td>
    </tr>
  </tbody>
</table>
