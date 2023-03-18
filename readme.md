To use `expand_contractions` function to expand contractions,

```python
from contu.contu import expand_contractions

string = "I'm going to this party."
expanded_string = expand_contractions(string, initial_case="uppercase")
print(expand_string)
```
This function takes a sentence as an input and replaces contractions in the sentence with their expanded forms using a dictionary of contractions and their expanded forms. The function also allows the user to choose the case of the output sentence, either lowercase or uppercase, with an optional argument.

For example, the contraction "I'm" will be expanded to "I am" and "you're" will be expanded to "you are".

```python
>>> from contu.contu import expand_contractions
>>> expand_contractions("I'm")
'I am'
>>> expand_contractions("I'm", initial_case='uppercase')
'I am'
>>> expand_contractions("I'm", initial_case='lowercase')
'i am'
```


The function `expand_contractions` first checks the initial case of the input sentence and sets the case of the output sentence accordingly. If the user passes the initial_case argument as 'lowercase' or 'uppercase', the function converts the dictionary of contractions to lowercase or uppercase, respectively, and then converts the input sentence to lowercase or uppercase, respectively.