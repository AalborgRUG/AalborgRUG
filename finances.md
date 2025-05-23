AalborgRUG finances
================
Ege Rubak
19 May, 2025

## Income

Only source of income so far is the sponsorship by R Consortium (and we
do not expect that to change anytime soon):

``` r
old <- options(stringsAsFactors = FALSE)
income <- data.frame(date = "2017-10-23",
                     text = "R Consortium",
                     DKK = 1106.86)
income[2,] <- data.frame("2018-06-27", "R Consortium", 1119.06)
income[3,] <- data.frame("2019-07-25", "R Consortium", 1173.02)
knitr::kable(income)
```

| date       | text         |     DKK |
|:-----------|:-------------|--------:|
| 2017-10-23 | R Consortium | 1106.86 |
| 2018-06-27 | R Consortium | 1119.06 |
| 2019-07-25 | R Consortium | 1173.02 |

## Expenses

Biggest expense is meetup.com where we started on a basic plan but had
to upgrade when we hit 50+ members. The subscription info I have from
meetup.com so far is:

- Your last payment of US\$29.94 was received on Sep 30, 2017.
- Your next payment of \$47.94 for a 6 month Unlimited plan will be
  charged on Mar 30, 2018.
- Your last payment of US\$47.94 was received on Apr 1, 2018.
- Your next payment of \$47.94 for a 6 month Unlimited plan will be
  charged on Sep 30, 2018.

**NOTE:** With the new R Consortium RUG Program the subscription is paid
for by R Consortium, so this expense will no longer appear.

The only expense we expect now is to drinks and snacks for meetups that
aren’t sponsored by anyone.

``` r
expenses <- data.frame(date = "2017-10-03", text = "meetup.com", DKK = 192.10)
expenses[2,] <- data.frame("2017-11-13", "Snacks and drinks", 340.85)
expenses[3,] <- data.frame("2017-12-04", "Foreign bank transfer fee", 35.00)
expenses[4,] <- data.frame("2018-04-04", "meetup.com", 295.09)
expenses[5,] <- data.frame("2018-06-27", "Foreign bank transfer fee", 30.00)
expenses[6,] <- data.frame("2018-10-01", "Snacks and drinks", 506.25)
expenses[7,] <- data.frame("2019-04-23", "Snacks and drinks", 521.08)
expenses[8,] <- data.frame("2019-07-25", "Foreign bank transfer fee", 30.00)
expenses[9,] <- data.frame("2019-11-10", "Snacks and drinks", 683.90)
expenses[10,] <- data.frame("2023-04-13", "Snacks and drinks", 299.40)
expenses[11,] <- data.frame("2025-05-14", "Snacks and drinks", 480)
knitr::kable(expenses)
```

| date       | text                      |    DKK |
|:-----------|:--------------------------|-------:|
| 2017-10-03 | meetup.com                | 192.10 |
| 2017-11-13 | Snacks and drinks         | 340.85 |
| 2017-12-04 | Foreign bank transfer fee |  35.00 |
| 2018-04-04 | meetup.com                | 295.09 |
| 2018-06-27 | Foreign bank transfer fee |  30.00 |
| 2018-10-01 | Snacks and drinks         | 506.25 |
| 2019-04-23 | Snacks and drinks         | 521.08 |
| 2019-07-25 | Foreign bank transfer fee |  30.00 |
| 2019-11-10 | Snacks and drinks         | 683.90 |
| 2023-04-13 | Snacks and drinks         | 299.40 |
| 2025-05-14 | Snacks and drinks         | 480.00 |

## Current status

At the moment it all boils down to:

``` r
(profit <- sum(income$DKK) - sum(expenses$DKK))
```

    ## [1] -14.73

Since we have a deficit we should be worried.

## Budget

No, we don’t have a budget. Fingers crossed.

``` r
options(old)
```
