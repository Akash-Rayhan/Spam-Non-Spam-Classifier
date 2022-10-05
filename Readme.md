• Downloaded examples of spam and ham from Apache SpamAssassin’s public
datasets.

• Unzipped the datasets and get familiarized  with the data format.

• Splited the datasets into a training set and a test set.

• Wrote a data preparation pipeline to convert each email into a feature vector.
The  preparation pipeline  transforms an email into a (sparse) vector
indicating the presence or absence of each possible word. For example, if all
emails only ever contain four words, “Hello,” “how,” “are,” “you,” then the email
“Hello you Hello Hello you” would be converted into a vector [1, 0, 0, 1]
(meaning [“Hello” is present, “how” is absent, “are” is absent, “you” is
present]), or [3, 0, 0, 2] if you prefer to count the number of occurrences of
each word.

• Added hyperparameters to  preparation pipeline to control
whether or not to strip off email headers, convert each email to lowercase,
remove punctuation, replace all URLs with “URL,” replace all numbers with
“NUMBER,”  remove stop words " a, an, the"  remove absurd single characters "'s" or even perform lemmatization 

• Then tried out  classifier
