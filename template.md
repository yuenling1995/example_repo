Simple document
================
Yuen
10/22/2021

it can also be a pdf/word document (the “output” section above)

I’m an R Markdown document!

# Section 1

Here’s a **code chunk** that samples from a *normal distribution*:

``` r
samp = rnorm(100)
length(samp)
```

    ## [1] 100

# Section 2

\#\#\#\#This is a sub title

I can take the mean of the sample, too! The mean is 0.0013204.

``` r
#the code above gives the code chunk name
library(tidyverse)
```

    ## ── Attaching packages ─────────────────────────────────────── tidyverse 1.3.1 ──

    ## ✓ ggplot2 3.3.5     ✓ purrr   0.3.4
    ## ✓ tibble  3.1.3     ✓ dplyr   1.0.7
    ## ✓ tidyr   1.1.3     ✓ stringr 1.4.0
    ## ✓ readr   2.0.1     ✓ forcats 0.5.1

    ## ── Conflicts ────────────────────────────────────────── tidyverse_conflicts() ──
    ## x dplyr::filter() masks stats::filter()
    ## x dplyr::lag()    masks stats::lag()

``` r
plot_df = tibble(
  x = rnorm(500, mean = 2, sd = 4),
  y = 3 - 4.2*x + rnorm(500)
)

ggplot(plot_df,aes(x=x,y=y)) + geom_point()
```

![](template_files/figure-gfm/plot%20example-1.png)<!-- -->

Here is a list:

*this is my first item *list needs to be at least 2 items \*third item

### table

| Col 1 | Col 2 |
|-------|-------|
| a     | b     |
| c     | d     |

> This is a block quote
