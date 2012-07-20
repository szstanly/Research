# Reproducible research
__________________________

[Reproducible research][] means other people can reproduce your results after reading you paper. So your paper should contain codes and data[^1] and others can run the program your provided in the paper using some statistcal software, for example, R. [Yihui][] writes the Knitr package[^2] to implement the idea of Reproducible research and it really make RR enjoyable and fun.

## Tools 

So it will become a fashion[^3] to write reports using Knitr in RStudio, because:

+ In RStudio, we can write in Markdown language and don't need to care about formating.

+ We can put the R code in the report and the result will display in the report automatically by R. Then people can reproduce our results independently.

+ We can write beautiful math equation in $LaTeX$ in RStudio.

__________________________

## Techniques

We can show the data management process and all the results to others and write beautiful math equation by using R and $LaTeX$ in RStudio.

### R code chunks

We can write the R code chunk in the following format to show the code to readers and the R will report the result of the code in the Report. [R Markdown][] has details for writing R code in RStudio. The following is an example:



```r
library(ggplot2)
qplot(hp, mpg, data = mtcars) + geom_smooth()
```

![plot of chunk md-cars-scatter](figure/md-cars-scatter.png) 


### Math equations in $LaTeX$ 

We can write math equation using $LaTeX$ in RStudio. There are two ways to write beautiful math equation:

+ Inline equations use `$equations$`.

+ Display equations `$$equations$$`.

Here is an inline equation: $x_t^2+y_t^2=r^2$, and the following is a display equation: $$ y_{it}=\beta_1x_{it}+\epsilon_{it}$$.  

______________________________________________________________________________________

[Reproducible research]: http://en.wikipedia.org/wiki/Reproducibility#Reproducible_research

[Yihui]: http://yihui.name/en/2012/06/enjoyable-reproducible-research/

[R Markdown]: http://www.rstudio.org/docs/r_markdown


[^1]: Or they can be downloaded from the internet.

[^2]: There are many packages in R to facilitate doing RR, see [CRAN Task View: Reproducible Research](http://cran.r-project.org/web/views/ReproducibleResearch.html).

[^3]: 阳志平:[为什么Markdown+R有较大概率成为科技写作主流？](http://www.yangzhiping.com/tech/r-markdown-knitr.html)
