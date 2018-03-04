# Statistical comparative analysis of Russian rap artists
## Intoroduction

This Jupyter Notebook uses Genius API and some data-analysis python libraries to analyse the vocabulary of modern Russian rappers.

## What did I find so far:
### Number of unique words per artist
I used 10000 words from each artist, from most popular songs, and compared how many words are unique, e.g. used only by this specific artist. The results are quite intersting, ranging from ~2000 (every 5th word you hear is only used by this artist) to ~500 (only every 20th word is unique).
![Uniq_words](/figs/unique_words.png)
### Number of self-referring words for each artists
This graph just looks at the proportion that words like I, me, mine make up in the lyrics. Again, artists range from up to 10%, mostly in the younger artists, to less than 5% in the older school.

![Self-words](/figs/self_love.png)

### Number of swear words for each artist

Same as the self-referring one, looks at the proportion of swear words in the vocabulary of an artists. Here we can see that some artists (very new and young artist Face) tops everyone else more than two-fold.


![Swear-words](/figs/swear_words.png)
___

### Correlations

It is quite obvious from the graph, that swearing, referring to yourself and the variety of vocabulary have a correlation, but just to check I did a Pearson statistical analysis on the datasets. And funnily enough, correlation coefficients were all astonishingly high:

#### Swearing and self-love

- Correlation coefficient:
0.91

- 2-tailed p-value:
2.92e-09

#### Swearing and vocabulary:

* Correlation coefficient:
0.88

* 2-tailed p-value:
4.32e-08

#### Self-love and vocabulary:

* Correlation coefficient:
0.97

* 2-tailed p-value:
1.07e-13
