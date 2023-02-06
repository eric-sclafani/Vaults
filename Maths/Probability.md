https://www.youtube.com/@DrTrefor

# The basics

- **`Probability`** - the chance of one event occuring out of all possible events. 

# Conditional Probability
- `Conditional probability` is the probability of an event **A** occuring given event **B** already occured:

  $P(A|B) = \dfrac{P(A \cap B)}{P(B)}$, A.k.a, probability of **A** `and` **B** occuring amonst all the possibilities of **B** occuring
  ![[cond_prob]]

## Examples

1. The % of adults who are men is **50%**. The % of adults who are men  AND an alcoholics is **2.25%**. What is the probability of being an alcoholic, given being a man?
	- Let A = alcoholic
	- Let b = man
	- $P(A \cap B) = 0.0225$
	-  $P(A|B) = \dfrac{P(A \cap B)}{P(B)} = \dfrac{0.0225}{0.5} = 0.045$


# Bayes theorem

`If` $P(A|B) = \dfrac{P(A \cap B)}{P(B)}$ , `then`   $P(B|A) = \dfrac{P(B \cap A)}{P(A)}$. In this case, $P(A \cap B)$ and $P(B \cap A)$ are equivalent. 
`Therefore:`
$P(A|B) = \dfrac{P(B|A)*P(A)}{P(B)}$

# Joint probability