# Brew to success (title subject to change) 
This project explores the factors in beers that lead to better reviews and can be seen as a manual to success.


distinction review (everything of a post) vs rating (number betwenn 1 -5)

## Project Proposal (Milestone 2)
Organize reviews in groups according to characteristics such as:
- type of beer reviewed
- country of residence of the user
- ...

Regarding the temporal aspect, the different groups can then be analysed across:
- the different months of the year
- the entire timeline of the reviews
- (per month?)
- ...

Whatever set of combinations of these two aspects is chosen can then yield recommendations on how to produce and launch a successful beer. Successfulness is measured by ratings and only the top X beers for a certain Group and Time are chosen.
Examples:
- For the group of type `Lambic` in `January` we only look at the beers `a`, `b` and `c` as they are considered the most successful with their average rating of 4.6, 4.58 and 4.52 accross all recorded januaries.
- For the group of type `Imperial IPA` in `2011` we only look at the beers `x`, `y` and `z` as they are considered the most successful with their average rating of 4.6, 4.58 and 4.52 across 2011.

We decided not to proceed with the `matched_beer` dataset initially supplied as merging the datasets of `BeerAdvocate` and `RateBeer` provides a more complete dataset.
