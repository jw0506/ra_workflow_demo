analyses example
================
JP
June 5, 2017

Why do I need to back up (e.g., "../" if my getwd() indicates that I am already in the proper folder)???

``` r
ds <- read_rds(file_mtcars)
```

``` r
ds %>% 
  ggplot(aes(x = wt, y = mpg)) +
  geom_boxplot(aes(group = cut_width(wt, 1)), varwidth = TRUE)
```

![](analyses_example_files/figure-markdown_github/unnamed-chunk-3-1.png)
