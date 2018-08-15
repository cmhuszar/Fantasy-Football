# Fantasy Football Auction Draft Strategy
A project on fantasy football.

##Project Motivation:
The term moneyball was made famous by a book and movie about the Oakland Athletics baseball team.  In short, it foccused on using analytical techniques to assemble a competitive baseball team for a low budget market team.  The purpose of this project is to apply the same general approach to fantasy football.

##Problem:  
Each year, fantasy football starts out with a draft.  In our league, the draft is an auction.  This means each team (8 teams total) get a $200 budget to bid on players.  Teams have nine starting positions (1 QB, 2 RB's, 3 WR's, 1 TE, 1 Defense/Special Teams, and 1 Kicker), and seven bench positions.  The goal of this analysis is to find a draft strategy that will maximize fantasy points and stay within the $200 budget.   

##Assumptions:

- This analysis only looks at 7 starting positions.  I don't evaluate defense and kickers.

- It doesn't account for risk.  Players get injured.  Some individuals or positions more than others.

- It takes a simplistic approach on byes and bench players.  Meaning, I'm assuming all other players drafted that are not     the 7 starting positions are done so at 1 each.  The logic is that bench players dont score points that count, and I have    to have to draft bench positions at some cost.

- I am assuming that the rankings or projections for this year are the best knowledge available.  Most team owners use this   as a way to determine value for players.

- I assume that the player projected rankings directly align with the spending patterns for each position in the previous     year.


##Structure:
1.  The data files used in the analysis are:

    Filename                          | Description
-------------                         | -------------
2018 Fantasy Football QB RB WR TE.csv | Data of 2017 fantasy football players stats and points for our league.
2017 Draft Results.csv                | Data of our 2017 draft results.
2017 ESPN PPR Projections Top 200.csv | For future analysis.
2018 ESPN PPR Projections Top 300.csv | For future analysis.

2.  Analysis is all performed in R using R Markdown.  To run, just change the directory references to where the two files are stored.

3.  Position Spending Optimization 2018.xlsx is an optimization solver through Excel that figures out the best roster based on the 2017 auction results and fantasy results.

##Next Steps
* Do optimization in R
* Add in risk
* Add web scraping for data generation
* Run on AWS
* Recreate using Python

    