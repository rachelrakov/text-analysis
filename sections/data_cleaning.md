# Data Cleaning 

Generally, however, our questions are more about topics rather than writing style. So, once we have a corpus (whether that is one text or millions), we usually want to clean and normalize it. Language is messy, and created for and by people, not computers. There is a lot of grammatical information in a sentence that a computer cannot use. For example, I could say to you `The house is burning.` and you would understand me. You would also understand if I say `house burn`. The first has more information about tense, and which house in particular, but the sentiment is the same either way. 

Usually, the computer works better with the second version (depending, of course, on your research question). In going from the first to the second, we removed the stop words (*the* and *is*), and normalized (removed punctuation and case) and lemmatized what was left (*burning* becomes *burn* - though we might have stemmed this, its impossible to tell from the example). This results in what is essentially a "bag of words," or a corpus of words without any structure. Again, this will be covered more in depth in the Machine Learning Tutorial, but for the time being, we just need to know that there is "clean" and "dirty" data. Sometimes our questions are about the clean data, but sometimes our questions are in the "dirt."

## Words into Numbers

In the next section, we are going to go through a series of methods that come built-in to NLTK that allow us to turn our words into numbers and visualizations. This is just scratching the surface, but should give you an idea of what is possible beyond just counting. 
