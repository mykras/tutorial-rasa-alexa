## happy path               <!-- name of the story - just for debugging -->
* greet
  - utter_greet
* mood_great               <!-- user utterance, in the following format: * intent{"entity_name": value} -->
  - utter_happy

## sad path 1               <!-- this is already the start of the next story -->
* greet
  - utter_greet             <!-- action of the bot to execute -->
* mood_unhappy
  - utter_cheer_up
* affirm
  - utter_happy

## sad path 2
* greet
  - utter_greet
* mood_unhappy
  - utter_cheer_up
* deny
  - utter_goodbye_console

## say goodbye
* goodbye
  - utter_goodbye

## bot challenge
* bot_challenge
  - utter_iamabot