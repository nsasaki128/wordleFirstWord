# Let's choose wordle first word
You can get a five-letter word for wordle first turn.
```
shuf -n 1 different_alphabet_five_letter_words.txt
```

## Look up dictionaries
If you want to know the meaning of the word, execute the commands below.

From https://www.dictionary.com/
```
shuf -n 1 different_alphabet_five_letter_words.txt | xargs -I{} sh -c 'open https://www.dictionary.com/browse/{} && echo {} is your first word'
```

From https://www.oxfordlearnersdictionaries.com/
```
shuf -n 1 different_alphabet_five_letter_words.txt | xargs -I{} sh -c 'open https://www.oxfordlearnersdictionaries.com/definition/english/{}?q={} && echo {} is your first word'
```

## Note
Original words are from http://www.gwicks.net/dictionaries.htm

ENGLISH - 194,000 words

We choose five letters words and also all the letters in these words are different.
