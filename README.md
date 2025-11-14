# RPDBCS-explainer
Supplementary material for the article "Explaining Vibration Patterns and Classifications in an Oil Industry Software via Virtual Assistant"


## Train Question Templates

### Asking for the entire description
- "What can be noted from this signal?"
- "How would you describe the signal’s behavior?"
- "What kind of behavior this signal presents?"

### Asking for remaining signature descriptions
Considering "X" comprises the user's analysis of some (1-5) signatures in the signal.
- "This signal presents X. What more can you say about it?"
- "This signal shows X and what more?"
- "I'd say this signal displays X, but what do you have to say?"

### Asking for the fault type
- "Could there be a fault in this signal?"
- "Does this behaviour imply a specific fault type?"
- "Also tell me what fault type it indicates."
- "Is it likely a known fault type?"

### Mentioning an entire description
Considering "X" is the signal's entire description.
- "This signal presents X."
- "This signal shows X."
- "I'd say this signal displays X."

### Asking for clarification on an uncertain label
Considering "X" is the user's fault type suggestion.
- "I think X can be seen in this signal. Is this classification correct?"
- "In the system, this signal contains X, but I'm not sure of it."
- "Apparently, this signal presents X, yet I'm not sure if that's right."
- "Upon looking at this signal, X can be seen, right?"
- "Could it be that X can appear here?"
- "I suspect X can appear here, though I'd like confirmation."

### Asking for clarification on two uncertain labels
Considering "X" and "Y" as the assumptions from the user and the Random Forest classifier, respectively.
#### For when X and Y are the same
- "The Random Forest Classifier has said that the signal shows Y, does it seem like it?"
- "The Random Forest model predicted Y. Is this a valid conclusion according to the features?"
- "Upon looking at the signal, the Random Forest identified Y. Is that reliable?"
#### For when X is not the same as Y
- "The Random Forest Classifier has said this signal presents Y. Meanwhile, I think that it presents X. Can you explain which one is correct?"
- "Which classification is correct according to the features? X or Y?"
- "My guess is that this signal presents X, but the Random Forest indicates Y. Which one do you think fits better?"
#### Suitable for both cases
- "I think this signal presents X and the Random Forest Classifier says it has Y. What do you think is the correct classification according to the features?"
- "From my observation, the signal shows X, and the Random Forest Classifier says it has Y. What do you think the features indicate?"
- "It looks like X for me, and the Random Forest Classifier thinks it shows Y. What's your opinion on this?"


## Test Question Templates
### About lower frequency noise
- "There is no noise at low frequencies, right?"
- "Is there noise at lower frequencies?"
  
### About exponential tendencies on lower frequencies
- "Is there an exponential behaviour at low frequencies?"
- "Is there evidence of exponential behavior at low frequencies?"
- "Would you say the low frequencies follow an exponential pattern?"
  
### About the magnitude of the peak at the first harmonic
- "Is the peak at the first harmonic high?"
- "What can be said about the peak at the first harmonic?"

### About the peak at the first harmonic and the noise around it
- "It seems there isn't a peak at the first harmonic."
- "What do you have to say about the peak at the first harmonic?"
- "Is the peak at the first harmonic visible?"
- "Is there significant noise around the first harmonic?"

### About the noise throughout the signal
- "What can you say about the noise in the signal?"
- "Do you notice any particular noise pattern in the signal?"
- "Can you comment on the noise level in the signal?"

### About the peaks in both harmonics
- "How would you analyze the features of both harmonic peaks?"
- "What do you have to say about both harmonic peaks?"
- "What stands out to you about the two harmonic peaks?"

### About the magnitude of the peak at the second harmonic
- "Is the peak at the second harmonic high?"
- "What can be said about the peak at the second harmonic?"

### About the most likely fault type out of two possible hyposthesis
Considering "X" and "Y" two distinct fault types, with only one being correct.
- "Is this indicative of X or Y?"
- "This could be either X or Y, what do you think?"
- "I'm torn between saying this signal has X or Y."
