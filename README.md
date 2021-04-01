# Article-Bias-Prediction

## Dataset
The articles crawled from www.allsides.com are available in the ```./data``` folder, along with the different evaluation splits.

The dataset consists of a total of 37,554 articles. Each article is stored as a ```JSON``` object in the ```./data/jsons``` directory, and contains the following fields:
1. **ID**: an alphanumeric identifier.
2. **topic**: the topic being discussed in the article.
3. **source**: the name of the articles's source *(example: New York Times)*
4. **source_url**: the URL to the source's homepage *(example: www.nytimes.com)*
5. **url**: the link to the actual article.
6. **date**: the publication date of the article.
7. **authors**: a comma-separated list of the article's authors.
8. **title**: the article's title.
9. **content_original**: the original body of the article, as returned by the ```newspaper3k``` Python library.
10. **content**: the processed and tokenized content, which is used as input to the different models.
11. **bias_text**: the label of the political bias annotation of the article (left, center, or right).
12. **bias**: the numeric encoding of the political bias of the article (0, 1, or 2).

The ```./data/splits``` directory contains the two types of splits, as discussed in the paper: **random** and **media-based**. For each of these types, we provide the train, validation and test files that contains the articles' IDs belonging to each set, along with their numeric bias label.

## Code
Under maintenance. To be available soon.

## Citation

```
@inproceedings{baly2020we,
  author      = {Baly, Ramy and Da San Martino, Giovanni and Glass, James and Nakov, Preslav},
  title       = {We Can Detect Your Bias: Predicting the Political Ideology of News Articles},
  booktitle   = {Proceedings of the 2020 Conference on Empirical Methods in Natural Language Processing (EMNLP)},
  series      = {EMNLP~'20},
  NOmonth     = {November},
  year        = {2020}
  pages       = {4982--4991},
  NOpublisher = {Association for Computational Linguistics}
}
```
