<!-- README.md is generated from README.Rmd. Please edit that file -->
Call \``meme` to add meme captions:

``` r
library(me2)
u <- "http://www.happyfamilyneeds.com/wp-content/uploads/2017/08/angry8.jpg"
meme(u, "code", "all the things!")
```

![](Figs/unnamed-chunk-2-1.png)

The `meme` output can be save as an object, and can be exported to file using `meme_save`:

``` r
u <- "http://news.china.com.au/wp-content/uploads/2016/04/640-841.jpeg"
x <- meme(u, "please", "tell me more", plot=FALSE)
x
meme_save(x, file="Figs/meme.png")
```

![](Figs/meme.png)

Users can `plot` the `meme` output and change the caption or other parameters in real time.

``` r
plot(x, size = 2, "happy friday!", "wait, sorry, it's monday", color = "firebrick", font = "Courier")
```

![](Figs/unnamed-chunk-4-1.png)
