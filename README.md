## Installation

All code was written in Python 3.6. Necessary dependencies are provided in `requirements.txt`.

## Project motivation

This project was inspired by Udacity Data Scientist Nanodegree mini project *"Write A Data Science Blog
 Post"*. I wanted to practice
  [CRISP-DM process](https://en.wikipedia.org/wiki/Cross-industry_standard_process_for_data_mining) 
  on  sports performance and betting data. For these reasons, I chose to investigate
   historical data of top basketball leagues in USA and Europe. Initially, I wanted to answer these 
   questions:

* Which are the most unprofitable bets?
* Are there any blind betting profitable strategies?
* What are the main differences between North America and Europe leagues?
* Do sports markets correct themselves overtime?
* Who are the most successful winners?

To answer these questions I scraped Oddsportal.com and wrote a blog post **[placeholder]**.

## Key observations

* Closing odds reflect true probabilities:

![fig 1](images/observed_prob_vs_implied_separate.png "Correlation plot")

* Randomly betting on closing odds is not profitable:

![fig 2](images/random_bet_simulations.png "Simulation results")

## File description

* `basketball_data_scraper.ipynb` notebook with data scraping code.
* `data_processing.ipynb` notebook with all data processing and analysis code.
* `geckodriver.exe` executable file for Morzilla Firefox.
* Folder `data` contains .csv files with scraped data:
  * `basketball_games.csv` scraped NBA and Euroleague 2013-2018 seasons data.
  * `NBA_20XX_20YY.csv` and `EURO_20XX_20YY.csv` asian handicap and totals (under/over X) for NBA and Euroleague 2013-2018 seasons games.
* Folder `images` contains various .png files.