# Investigating the influence of history on the movie industry
## Team: ADAcADAbra
DEMIRTAS Enes Eray\
MAILLARD Alexandre Benjamin\
SIRIPATTHITI Punnawat\
ZEMP Manuel Nicolas

## Abstract
Literature is a mirror of history. At least some forms of literature can be interpreted as a memory of the past. Authors write about challenges, problems and fates of individuals and society, which reflects their perspective of the times they’re living in, even though sometimes no evident connection to a specific historical moment needs to exist. Can such a statement be adapted to other media formats, like movies, as well? Surely there exist a lot of movies, which purely serve the purpose to entertain. But, as in literature, there could be some degree of reflection of contemporary events and developments hidden in the plots or characteristics of a movie, a reflection of history.

In this project, we try to investigate that subject by analysing the data in the dataset CMU Movie Summary Corpus. We determine through different tests whether specific events and developments in history have had an influence on various parameters of the movie industry, like the plots of movies or the types of movies that were produced. 

## Our data story
We are choosing a set of historical events and developments, which have had a major impact on the world. These events are all unique and their possible influences on the movie industry can be derived from their characteristics. We test the data on whether a change in these expected domains of the movie industry is measurable inside a reasonable time frame related to the event. By testing several independent events we can detect a pattern on if and how history is indeed reflected in movies. 

History is written by different kinds of changes, which we categorise like this: abrupt changes and slow developments. Abrupt changes are single-time events, which happened for a short period and changed the world immediately. An example of an abrupt change is the end of World War II. Slow developments take years to show a tangible effect. As they are not necessarily determined by single-time events, but rather by the mindsets and attitudes of people and society which are changing slowly over time. An example of slow development is gender neutrality. We include in the analysis the distinction between these two types of historical events and try to determine if one of them has a greater influence on the movie industry than the other.

## Research Questions
Investigating the influence of history on the movie industry: A) Is there a measurable influence of history on the movie industry? How strong is this influence? B) Can we say that detected changes in movies are influenced by history, or are these changes the natural development of the movie industry anyways? C) Are abrupt changes or slow developments more impactful? D) Are there specific genres that are affected more or less? E) Are there categories of history subjects that are influencing more?

## Additional datasets: 
No additional data sets are required for this project, however, information on history had to be collected. Inspired by this website (https://eu.usatoday.com/story/money/2020/09/06/the-worlds-most-important-event-every-year-since-1920/113604790/) a series of historical events has been chosen: 
* 1945: World War II Ends
* 1969: Moon Landing
* 1979: Energy crisis and, as a follow-up: Early 1980s Recession (https://en.wikipedia.org/wiki/List_of_economic_crises)
* 1997: Machine Tops Chess Champ
* 2001: 9/11
* 2005: Katrina Overwhelms New Orleans

These events all belong to our definition of abrupt changes. In addition, they represent historical developments of different categories: The end of WWII and 9/11 are events related to war, the Moon Landing and the machine topping a chess champion are scientific breakthroughs, the energy crisis and the 1980s recession are economical and the hurricane Katrina is a natural catastrophe. This diversity is interesting for our analysis, as we might get more or less influence from different categories. \
For the slow developments, we decided to attack the following history subjects: 
* gender neutrality
* human rights
* racism
All of the above events have to be characterised in order to be able to detect movies that are concerned with the subjects. In the notebook, there is a description of how we plan on performing this characterisation, along with two examples (WWII and gender neutrality). 

## Methods
* Step 1 Data preparations (milestone P2): Analyse the data, determine what is of interest to our analysis, check for data errors (data-scraping), and prepare the dataframes for the analysis.
* Step 2 Determine historical events and define their unique characteristics. 
* Step 3 Perform the analysis according to plan.
  * Identify the set of movies of interest at the time of reference, divided into a training set and a validation set. The value that will be used as the dependent variable in a linear formula is frequency, absolute number, or change (to be determined later)
  * Identify all relevant independent variables (a.k.a feature extraction) to formulate the linear formula by using a correlation matrix and leave-one-out cross-validation. Try to address any collinearity.
  * Perform a multiple regression analysis and get the predicted values for the time of impact.
  * ValidateDefine null hypothesis: the real values correlate with the expected values, meaning there are no significant changes in the dataset. Then perform hypothesis testing
  * Evaluate the results by using residual plot to address heteroscedasticity etc.
* Step 4 Put the results together and come up with a conclusion. Document everything in a presentable manner.
Check the notebook for more details on each step. 

## Proposed timeline and organisation within the team
18/11/2022: Step 1, parts of Step 2 (everybody)\
09/12/2022: Step 2 (everybody)\
16/12/2022: Step 3 (mainly Alex, Kla, and Eray)\
23/12/2022: Step 4 (mainly Manu, then everybody)

## Questions for TAs: 
About the number of events, we are investigating: Since we do not yet exactly know how much work we will face for each event, we decided to go with not too many for the moment. Maybe we’ll manage to add more events and with that, give more credibility to our conclusion. Do you agree with this procedure?
