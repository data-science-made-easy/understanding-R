# R course
This course is an introduction into R for starters in data science.

## Installation and basics
First install R or RStudio and get familiar with R's basics, following [this link](https://cran.r-project.org/doc/contrib/Torfs+Brauer-Short-R-Intro.pdf "Get to know the basics").

## Regular functions
In R you can write your own functions, e.g.:

```R
factorial <- function(n) {
  result <- 1
  if (0 < n) {
    for (i in 1:n) {
      result <- result * i
    }
  }
  return(result)
}
```

## Recursive functions
The factorial function can be implemented in a recursive way, too.

```R
factorial <- function(n) {
  if (0 == n) { # base
    return(1)
  } else { # recursive step
    return(n * factorial(n - 1))
  }
}
```
