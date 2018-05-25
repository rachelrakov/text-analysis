# Positioning Words

In many ways, `concordance` and `similar` are heightened word searches that tell us something about what is happening near the target words. Another metric we can use is to visualize where the words appear in the text. In the case of *Moby Dick*, we want to compare where "whale" and "monster" appear throughout the text. In this case, the text is functioning as a list of words, and will make a mark where each word appears, offset from the first word. We will *pass* this *function* a *list* of *strings* to plot. This will likely help us develop a visual of the story - where the whale goes from being a whale to being a monster to being a whale again. In the next cell, type:

	text1.dispersion_plot(["whale", "monster"])

A graph should appear with a tick mark everywhere that "whale" appears and everywhere that "monster" appears. Knowing the story, we can interpret this graph and align it to what we know of how the narrative progresses. If we did not know the story, this could give us a picture of the narrative arc.

Try this with text2, *Sense and Sensibility*. Some relevant words are "marriage," "love," "home," "mother," "husband," "sister," and "wife." Pick a few to compare. (You can compare an unlimited number, but it's easier to read a few at a time.)

NLTK has many more functions built-in, but some of the most powerful functions are related to cleaning, part-of-speech tagging, and other stages in the text analysis pipeline (where the pipeline refers to the process of loading, cleaning, and analyzing text).
