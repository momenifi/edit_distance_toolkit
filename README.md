# Analyzing Text Similarity and Distortion Using Edit Distance
## Description
This method calculates how similar or different two texts are by measuring the "edit distance," which counts the changes (insertions, deletions, substitutions, or transpositions) needed to transform one text into another. It includes 3 variations: simple edit distance, Levenshtein distance, and Damerau-Levenshtein distance, applied at both word and character levels. Additionally, the method can distort text by randomly applying edit operations, which is useful for anonymizing data. Social scientists can use this tool to compare definitions of concepts across disciplines, analyze variations in language between dialects, or study differences in how various media outlets report news.
 It has the following operations:

- simple edit distance between two texts (at word level)
- simple edit distance between two texts (at character level)
- levenshtein edit distance (with substitution cost 2) between two texts (at word level)
- levenshtein edit distance (with submistution cost 2) between two texts (at character level)
- damerau-levenshtein edit distance between two texts (at word level)
- demarau-levenshtein edit distance between two texts (at character level)
- distorting or randomizing text for given number of spins of randomly picked operations (insertion, deletion, substitution and transposition)

The methods are defined in `utils.py` and are called on sample tweets from the notebook `text_edit_distance.ipynb`

The method in plain Python without any package installation and therefore, preserving the environment or the `requirements.txt` file is not required. Random seeds are defined to have predictable random numbers for reproducibility.

## Keywords
edit distance, randomizing text, levenshtein edit distance, damerau-levenshtein

## Use cases
1. Evaluating Media Reporting:
Social scientists can compare how different media outlets report the same news story by analyzing the similarities and differences in wording, framing, and tone.

2. Text Anonymization for Privacy:
When analyzing datasets with sensitive information, researchers can use the text distortion feature to anonymize personal details without losing the overall structure of the text.

## How to use
- run jupyter using command `jupyter lab` or `jupyter notebook`
- execute the notebook cells to call all methods defined in `utils.py` on same texts

## Sample input (For example to tweets)

```
tweet1 = "Excited to share our latest research on AI and its impact on social sciences! Leveraging data for better insights"
tweet2 = "Thrilled about our new findings on how AI transforms social science research. Innovation meets impact!"
```

## Sample output

```
simple edit distance at character 71, at word 16
levenshtein edit distance at character 109, at word 26
...
```

### Contact Details
Taimoor Khan (taimoor.khan@gesis.org)
