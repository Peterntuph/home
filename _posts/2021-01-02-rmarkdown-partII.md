---
layouts: archive
classes: wide
permalink: /Rmarkdown-partII
title: " R Markdown Quick Tutorial (Part II)"
---

In the [previous post]( https://peterntuph.github.io/home/Rmarkdown-partI ), I have demonstrated five simple steps to construct your own R Markdown document. In this post, I am going to share some useful tips for adding mathematical expressions, inline graphs or tables to represent your results with clarity.

## 1. Inline Code

To add explanations to our R Markdown, we sometimes need to refer to the objects we created in the R Studio environment. Therefore, just simply insert its name with ` `` `. The results will appear as text without code.

For example,
> According to the Table.1, the overall five-year survival rate for colon cancer patients is `  colon_five_year ` <br>

Results:
> According to the Table.1, the overall five-year survival rate for colon cancer patients is 0.63 <br>

## 2. Mathematical expressions

Typing mathematical expressions in R markdown is the same in [LATEX]( https://www.latex-project.org/). The following table lists some frequently used symbols or mathematical operators.

| Input | Output | Input | Output |
|:------:|:-----:|:-------:|:-----:|
| \langle | ![formula](https://render.githubusercontent.com/render/math?math=\langle) | \rangle | ![formula](https://render.githubusercontent.com/render/math?math=\angle) |
| \lbrace | $\lbrace$ | \rbrace | $ \rbrace $ |
| \sum | $\sum$ | \lim | $ \lim $ |
| \alpha | $ \alpha $ | \beta | $ \beta $ |
| \gamma | $ \gamma $ | \delta | $ \delta $ |
| \lambda | $ \lambda $ | \mu | $ \mu $ |

For complete lists of mathematical expressions in LATEX format, Please visit the [The Comprehensive LaTeX Symbol List]( https://mirror-hk.koddos.net/CTAN/info/symbols/comprehensive/symbols-a4.pdf).

Moreover, there are two writing modes for mathematical expressions in R markdown: the inline mode and the display mode. The first one is to add formulas that exist as a part of the text. The second one is to write expressions that are put on separate independent lines.

* Let's see an example of the **inline** mode:
> The formula for the mean is $ \overline{X} = \frac{\sum{X}}{n} $ where x represents each of the values in the data set.

Result: 
![inline]( https://raw.githubusercontent.com/Peterntuph/home/master/_pics/rmarkdown2_1.png)

* The example of **displayed** mode:

> The formula for the mean is $$ \overline{X} = \frac{\sum{X}}{n} $$ where x represents each of the values in the data set.

Result: <br>
![displayed]( https://raw.githubusercontent.com/Peterntuph/home/master/_pics/rmarkdown2_2.png)

## 3. Graphs

We have mentioned a lot of useful syntax in Markdown in my [first post]( https://peterntuph.github.io/home/my-first-post). The syntax is nearly the same in creating images in R Markdown & Markdown

For example: 
> `![ Pythagora’s theorem]( https://cdn.zmescience.com/wp-content/uploads/2017/05/Pythagorean-Theorem.jpeg)`

Result:
![ Pythagora’s theorem]( https://cdn.zmescience.com/wp-content/uploads/2017/05/Pythagorean-Theorem.jpeg){width=50%}

## 4. Table

We use `|`, `-`, and `enter` to create table with Markdown.

1. The first row has to be the “header row”, which determines the number of columns in this table.
2. The second row must contain `-` separating pipes `|`.
3. The pipes `|` separate each column.

For example: 

`| header 1 | header 2 |` <br>
`|---|---|` <br>
`|row 1 col 1 | row 1 col 2|` <br>
`|row 2 col 1 | row 2 col 2|` <br>

Result:

| header 1 | header 2 |
|---|---|
|row 1 col 1 | row 1 col 2|
|row 2 col 1 | row 2 col 2|

## Reference
1. [The most beautiful and important mathematical equations]( https://www.zmescience.com/other/feature-post/mathematical-equations-beautiful-30112018/)
2. [Mathematical Expressions]( https://www.overleaf.com/learn/latex/Mathematical_expressions)

Written in January 2nd, 2021
