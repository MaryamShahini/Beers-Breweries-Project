Introduction:

Objective:

The objective is to analyze the available Breweries and Beers data sets
in order to understand the

Import .csv data sets from local computer

    Beers <- read.csv(file="C:/Users/R900255/Desktop/Uni/Doing DS/Beers.csv")
    Breweries <- read.csv(file="C:/Users/R900255/Desktop/Uni/Doing DS/Breweries.csv")

1. How many breweries are present in each state?
------------------------------------------------

    Brew.per.State  <- aggregate(rep(1, length(paste0(Breweries$State))),
                                 by=list(Breweries$State), sum)
    Brew.per.State

    ##    Group.1  x
    ## 1       AK  7
    ## 2       AL  3
    ## 3       AR  2
    ## 4       AZ 11
    ## 5       CA 39
    ## 6       CO 47
    ## 7       CT  8
    ## 8       DC  1
    ## 9       DE  2
    ## 10      FL 15
    ## 11      GA  7
    ## 12      HI  4
    ## 13      IA  5
    ## 14      ID  5
    ## 15      IL 18
    ## 16      IN 22
    ## 17      KS  3
    ## 18      KY  4
    ## 19      LA  5
    ## 20      MA 23
    ## 21      MD  7
    ## 22      ME  9
    ## 23      MI 32
    ## 24      MN 12
    ## 25      MO  9
    ## 26      MS  2
    ## 27      MT  9
    ## 28      NC 19
    ## 29      ND  1
    ## 30      NE  5
    ## 31      NH  3
    ## 32      NJ  3
    ## 33      NM  4
    ## 34      NV  2
    ## 35      NY 16
    ## 36      OH 15
    ## 37      OK  6
    ## 38      OR 29
    ## 39      PA 25
    ## 40      RI  5
    ## 41      SC  4
    ## 42      SD  1
    ## 43      TN  3
    ## 44      TX 28
    ## 45      UT  4
    ## 46      VA 16
    ## 47      VT 10
    ## 48      WA 23
    ## 49      WI 20
    ## 50      WV  1
    ## 51      WY  4