[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-718a45dd9cf7e7f842a935f5ebbe5719a5e09af4491e668f4dbf3b35d5cca122.svg)](https://classroom.github.com/online_ide?assignment_repo_id=12557331&assignment_repo_type=AssignmentRepo)
# Quicksort Pivots

in the lectures I only briefly mentioned strategies for determining a good pivot
for quicksort. The implementation on the slides simply picks the leftmost
element in the part of the array that we consider as a pivot. I also mentioned a
few other ways of picking a good pivot, e.g. randomly.

Median-of-three is also a good way of picking a pivot -- inspect the first,
middle, and last elements of the part of the array under consideration and
choose the median value. Using the probabilities for picking a pivot in a
particular part of the array (in the same way as we did on slide 34), argue
whether this method is more or less (or equally) likely to pick a good pivot
compared to simply choosing the first element. Assume that all permutations are
equally likely, i.e. the input array is ordered randomly.

Your answer must derive probabilities for choosing a good pivot and
quantitatively reason with them.

Add your answer to this markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.


## My Response

When it comes to choosing the best pivot for a quicksort algorithm there are two qualities you look for in a pivot. The first quality is a pivot which is easy to choose, and the second is one that pivots to the middle of the array. So when choosing to use a random pivot or choosing the median of three we have to consider a few factors to find which is better. The way I see it in order to figure out which is better we need to find out which one has a higher chance of being a good pivot.

The way I to describe a good pivot would be the middle half of the array. So a good pivot would be greater than 1/4 of the array but less than 3/4 of the array. So all we need to do is figure out which one has a better chance of being in the middle of the array. The random one is easy since it has a 1 in four chance of being a good choice, but the middle of three is a bit harder to figure out. So to figure out the odds of the choice to being good I just came up with all possible combinations and then counted all the times that a good pivot would be in the middle. This gave me a 3/5 chance to pick a good pivot. Therefore I believe picking the median of three numbers leads to a better outcome more of the time.
