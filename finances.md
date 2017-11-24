AalborgRUG finances
================
Ege Rubak
November 24, 2017

Income
------

Only source of income so far is the sponsorship by R Consortium (and we do not expect that to change anytime soon):

``` r
income <- data.frame(date = "2017-10-23",
                     text = "R Consortium",
                     DKK = 1106.86)
knitr::kable(income)
```

| date       | text         |      DKK|
|:-----------|:-------------|--------:|
| 2017-10-23 | R Consortium |  1106.86|

Expenses
--------

Biggest expense is meetup.com where we started on a basic plan but had to upgrade when we hit 50+ members. The subscription info I have from meetup.com so far is:

-   Your last payment of US$29.94 was received on Sep 30, 2017.
-   Your next payment of $47.94 for a 6 month Unlimited plan will be charged on Mar 30, 2018.

Besides this expense every six months we only expect expenses to drinks and snacks for meetups that aren't sponsored by anyone.

``` r
expenses <- data.frame(date = "2017-10-03", text = "meetup.com", DKK = 192.10)
expenses[2,] <- data.frame("2017-11-13", "Snacks and drinks", 340.85)
knitr::kable(expenses)
```

| date       | text              |     DKK|
|:-----------|:------------------|-------:|
| 2017-10-03 | meetup.com        |  192.10|
| 2017-11-13 | Snacks and drinks |  340.85|

Current status
--------------

At the moment it all boils down to:

``` r
(profit <- sum(income$DKK) - sum(expenses$DKK))
```

    ## [1] 573.91

Since we have a profit we are all happy.

Budget
------

No, we don't have a budget. Fingers crossed.
