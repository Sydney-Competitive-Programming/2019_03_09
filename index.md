The leaderboard
---------------

``` r
df = data.table::fread("data.csv")
df
```

    ##      username github       team pts p1s p2s p3s p1g p2g p3g p1e p2e p3e np
    ## 1: David Guan     NA David Guan  NA   1  NA  NA  NA  NA  NA  NA  NA  NA NA
    ##    num_attendees
    ## 1:            10

Plots
-----

You can also embed plots, for example:

    ## PhantomJS not found. You can install it with webshot::install_phantomjs(). If it is installed, please make sure the phantomjs executable can be found via the PATH variable.

<!--html_preserve-->

<script type="application/json" data-for="htmlwidget-e3c43b19f85d795d4226">{"x":{"filter":"none","data":[["1"],["David Guan"],["NA"],[10],[1]],"container":"<table class=\"display\">\n  <thead>\n    <tr>\n      <th> <\/th>\n      <th>team<\/th>\n      <th>github<\/th>\n      <th>pts<\/th>\n      <th>rank<\/th>\n    <\/tr>\n  <\/thead>\n<\/table>","options":{"columnDefs":[{"className":"dt-right","targets":[3,4]},{"orderable":false,"targets":0}],"order":[],"autoWidth":false,"orderClasses":false}},"evals":[],"jsHooks":[]}</script>
<!--/html_preserve-->

``` r
barplot(summ$pts, xlab = summ$team)
```

![](index_files/figure-markdown_github/plot-1.png)
