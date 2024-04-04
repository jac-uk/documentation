---
nav_exclude: true
---
# Working Preferences

## Version 2

### Configration in `exercise` (and `vacancy`) document

The are three places where working preference questions are asked:

 - Location preferences are stored in `exercise.locationPreferences`
 - Jurisdiction preferences  are stored in `exercise.jurisdictionPreferences`
 - Additional working preferences are stored in `exercise.additionalWorkingPreferences`

Each of these places allows multiple questions to be configured and there are three types of questions available, stored in `questionType`:

 - Single choice
 - Multiple choice
 - Ranked choice

As well as type of question there are a number of other configuration options such as:

 - whether the question is mandatory
 - how many answers should be selcted by the candidate
 - where the answers come from (`answerSource`)



### Answers provided in `application` document

Candidates are asked working preferences questions on their application form and their answers are stored in their `application` document in the following fields:

 - `application.locationPreferences`
 - `application.jurisdictionPreferences`
 - `application.additionalWorkingPreferences`

Answers are stored in these fields in a map, using the question ID as the key and the answer ID as the value(s). The shape of the data stored for each question is slightly different for each of the question types

For example the answers for three questions (one each of type single choice, multiple choice and ranked choice) might look as follows:

```
{
  "id1": "aid1",
  "id2": ["aid2", "aid3"],
  "id3": { "aid1": 1, "aid3": 2 }, 
}
```


#### Single choice answers

These questions have multiple answers where the user is expected to choose one (and only one) answer.
The answers are typically presented as radio buttons.

##### Data type for answers: `String`
e.g. 
```
"id1": "aid2"
```


#### Multiple choice answers

These questions have multiple answers where the user can choose any number of answers.
The answers are typically presented as checkboxes.

##### Data type for answers: `Array`
e.g. 
```
"id1": ["aid1", "aid3"]
```

#### Ranked choice

These questions have multiple answers. The user chooses answers and assigns each chosen answer a rank.
The answers are currently presented as checkboxes with rank dropdowns alongside.

##### Data type for answers: `Object`
An object containing the chosen answers as keys and the rank as the values, as follows:
e.g. 
```
"id1": {
  "aid1": 1,
  "aid3": 2
}
```

### Displaying answers

In order to display the answers a candidate has selected we need to utilise both the `application` document and the `exercise` (or `vacancy`) document.

 - `application` gives us the answers entered by the candidate
 - `exercise` gives us the configuration for the question 

Note that `application` stores IDs for the questions and selected answers only therefore we need the `exercise` in order to locate the text to display for the question and selected answer(s).


---

## Version 1

Previously location and jurisdiction could each have up to one question configured. These questions were stored in the following fields:

 - `exercise.locationQuestion`
 - `exercise.locationQuestionType`
 - `exercise.locationQuestionAnswers`
 - `exercise.jurisdictionQuestion`
 - `exercise.jursidictionQuestionType`
 - `exercise.jursidictionQuestionAnswers`
