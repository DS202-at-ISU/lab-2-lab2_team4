
<!-- README.md is generated from README.Rmd. Please edit the README.Rmd file -->

# Lab report \#1

Follow the instructions posted at
<https://ds202-at-isu.github.io/labs.html> for the lab assignment. The
work is meant to be finished during the lab time, but you have time
until Monday evening to polish things.

Include your answers in this document (Rmd file). Make sure that it
knits properly (into the md file). Upload both the Rmd and the md file
to your repository.

All submissions to the github repo will be automatically uploaded for
grading once the due date is passed. Submit a link to your repository on
Canvas (only one submission per team) to signal to the instructors that
you are done with your submission.

1.  There are the following 16 variables: Parcel ID, Address, Style,
    Occupancy, Sale Date, Sale Price, Multi Sale, YearBuilt, Acres ,
    TotalLivingArea, Bedrooms, FinishedBsmtArea (sf), LotArea(sf), AC,
    FirePlace, and Neighborhood. After running “?ames” we were able to
    get a description of each variable. We are anticipating that
    numerically price will be in the thousands, or hundreds of
    thousands, addresses within Ames zipcodes (shouldn’t be too many
    options), year can range from the first house built in ames (~200
    years prior) until 2024, bedrooms will be a single digit value, some
    are boolean variables (fireplace, finished basement, ac), lot area
    will be measured in acres and will be in the hundreds or more.

``` r
library(classdata)
data(Ames)
```

    ## Warning in data(Ames): data set 'Ames' not found

``` r
?(ames)
```

    ## starting httpd help server ... done
