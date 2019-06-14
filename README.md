# ETL--Urban Dictionary

# Background

This dataset contains 2.6 million words from Urban Dictionary.com

Source: https://www.urbandictionary.com

Dataset: https://www.kaggle.com/therohk/urban-dictionary-words-dataset

Format: CSV


# Proccess

Extract:

word_id - unique id for urban dictionary api

word

up_votes/ thumbs up count as of may 2016

down_votes/ thumbs down count as of may 2016

author

definition


Transform:

Checked if there was any blank definitions and deleted. There were 188 blank definitions that I removed.

Removed duplicates for word_id,word, author, and definitions

Removed duplicate words and meanings

Authored most contributed


Load:

Load to Postgree database using SQLalchemy.



