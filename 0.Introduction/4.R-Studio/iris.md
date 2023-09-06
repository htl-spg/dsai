Fisher’s Iris Dataset
================
rkofler
2023-08-28

## IRIS

<figure>
<img
src="https://raw.githubusercontent.com/htl-spg/dsai/iris/0.Introduction/4.R-Studio/images/iris_grw.jpg"
style="height:20.0%" alt="Iris, Weinviertel" />
<figcaption aria-hidden="true">Iris, Weinviertel</figcaption>
</figure>

## Loading data (iris flowers) from an included dataset

loading a dataset (package ‘datasets’ is a base package)

`library('datasets')`

show table’s headers

`head(iris)`

``` head(iris)
  Sepal.Length Sepal.Width Petal.Length Petal.Width Species
1          5.1         3.5          1.4         0.2  setosa
2          4.9         3.0          1.4         0.2  setosa
3          4.7         3.2          1.3         0.2  setosa
4          4.6         3.1          1.5         0.2  setosa
5          5.0         3.6          1.4         0.2  setosa
6          5.4         3.9          1.7         0.4  setosa
```

## show data structure

`str(iris)`

``` str(iris)
'data.frame':   150 obs. of  5 variables:
 $ Sepal.Length: num  5.1 4.9 4.7 4.6 5 5.4 4.6 5 4.4 4.9 ...
 $ Sepal.Width : num  3.5 3 3.2 3.1 3.6 3.9 3.4 3.4 2.9 3.1 ...
 $ Petal.Length: num  1.4 1.4 1.3 1.5 1.4 1.7 1.4 1.5 1.4 1.5 ...
 $ Petal.Width : num  0.2 0.2 0.2 0.2 0.2 0.4 0.3 0.2 0.2 0.1 ...
 $ Species     : Factor w/ 3 levels "setosa","versicolor",..: 1 1 1 1 1 1 1 1 1 1 ...
```

`?iris`

    Description:
    This famous (Fisher's or Anderson's) iris data set gives the
    measurements in centimeters of the variables sepal length and
    width and petal length and width, respectively, for 50 flowers
    from each of 3 species of iris.  The species are _Iris setosa_,
    _versicolor_, and _virginica_.

## Classification of unknown data

- data screening
- classification of a flower

## data summary - get a quick overview

``` r
# summary(iris)
```

``` summary(iris)
  Sepal.Length    Sepal.Width     Petal.Length    Petal.Width   
 Min.   :4.300   Min.   :2.000   Min.   :1.000   Min.   :0.100  
 1st Qu.:5.100   1st Qu.:2.800   1st Qu.:1.600   1st Qu.:0.300  
 Median :5.800   Median :3.000   Median :4.350   Median :1.300  
 Mean   :5.843   Mean   :3.057   Mean   :3.758   Mean   :1.199  
 3rd Qu.:6.400   3rd Qu.:3.300   3rd Qu.:5.100   3rd Qu.:1.800  
 Max.   :7.900   Max.   :4.400   Max.   :6.900   Max.   :2.500  
       Species  
 setosa    :50  
 versicolor:50  
 virginica :50
```

## Visualize data - the boxplot

``` r
boxplot(iris)
```

![](iris_files/figure-gfm/boxplot-1.png)<!-- -->
