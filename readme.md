# Wordle Study
This repository contains the algorithms used to conduct research on optimal Wordle algorithms as well as their results. Two algorithms representing two distinct approaches to the Wordle game are present.

## Masker
Titled `Wordle Player.ipynb`. This algorithm works by narrowing down the list of possible words. Of those possible words, the algorithm uses a primitive, unsophisticated function to determine which is most likely to narrow the list of possible words by the greatest margin (yield the greatest amount of novel information), selecting that word as its guess. All Masker's guesses will be possible correct words (compatible with the known information). As such, it **is** compatible with Wordle's *Hard Mode*.

## Greedy
Titled `Wordle Greedy.ipynb`. This algorithm takes a different approach to Wordle. Instead of repeatedly guessing valid words, Greedy attempts to guess the word that will yield the greatest amount of novel information (even if the known information suggests the guessed word cannot possibly be correct). **As Greedy is still a WIP, this is currently the extent of Greedy's functionality. All other features are being developed and will be implemented soon.** When Greedy is on its last guess, or when it reaches a certain *confidence threshold*, it will guess what it believes the correct answer to be. Since Greedy may guess words that are known to be incorrect, it **is not** compatible with Wordle's *Hard Mode*.
