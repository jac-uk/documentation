---
nav_exclude: true
---
# Working Preferences Answers

There are three types of questions for working preferences:

 - Single choice
 - Multiple choice
 - Ranked choice

There are typically multiple questions configured therefore answers to those questions are stored in a map using the question title as the key, as follows:

```
{
  "Question 1 title": "Answer 1",
  "Question 2 title": ["Answer 2", "Answer 3"],
  "Question 3 title": { "Answer 1": 1, "Answer 3": 2 }, 
}
```


## Single choice

These questions have multiple answers where the user is expected to choose one (and only one) answer.
The answers are typically presented as radio buttons.

### Data type for answers: `String`
e.g. 
```
"Question 1": "Answer 2"
```


## Multiple choice

These questions have multiple answers where the user can choose any number of answers.
The answers are typically presented as checkboxes.

### Data type for answers: `Array`
e.g. 
```
"Question 1": ["Answer 1", "Answer 3"]
```

## Ranked choice

These questions have multiple answers. The user chooses answers and assigns each chosen answer a rank.
The answers are currently presented as checkboxes with rank dropdowns alongside.

### Data type for answers: `Object`
An object containing the chosen answers as keys and the rank as the values, as follows:
e.g. 
```
"Question 1": {
  "Answer 1": 1,
  "Answer 3": 2
}
```

