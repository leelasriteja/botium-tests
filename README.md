# botium-tests
Sample botium scrips to run against Google Dialogflow

refer - https://chatbotsmagazine.com/3-steps-setup-automated-testing-for-google-assistant-and-dialogflow-de42937e57c6

Validate the configuration by running Botium in “emulator”mode — it will connect to your Dialogflow Agent and provides a simple chat interface in the terminal:

> botium-cli emulator

To run tests(as configures in package.json):
> npm run test

This has working demo of botium with bindings and botium emulator integrated with dialogflow!

To point out the convo file:

> export BOTIUM_CONVOS=/Users/leela/Desktop/botium_trial_three/spec/convo

To print env variables

> printenv

To install mochawesome

> npm install --save-dev mochawesome

If your terminal scroll doesn't work, try:

> reset

To view the report generated using our mocha test runner, you can go to "mochawesome-report/mochawesome.html" and open in chrome or any of your favourite browsers to view the report!

Which would look something like below,

<img width="1415" alt="Screen Shot 2023-05-18 at 6 27 19 PM" src="https://github.com/leelasriteja/botium-tests/assets/29068723/a7e1e88c-ef41-4f71-8233-ed594a902aac">

Some other useful references:

To connect to Dialogflow agent and create intents - refer https://www.pragnakalp.com/botium-setup-and-test-case-generation-for-dialogflow-agent/

My Google Dialogflow urls:

https://dialogflow.cloud.google.com/#/agent/testone-i9nj/intents

https://cloud.google.com/dialogflow/es/docs/entities-overview
https://cloud.google.com/dialogflow/es/docs/intents-overview
https://dialogflow.cloud.google.com/cx/projects/testone-i9nj/locations
https://cloud.google.com/dialogflow
https://cloud.google.com/dialogflow/docs/
https://chatbotsmagazine.com/3-steps-setup-automated-testing-for-google-assistant-and-dialogflow-de42937e57c6. **imp**

https://unpkg.com/browse/botium-connector-dialogflow@0.0.10/README.md
https://www.pragnakalp.com/botium-setup-and-test-case-generation-for-dialogflow-agent/



Dialogflow refs:

https://dialogflow.cloud.google.com/#/agent/testone-i9nj/editIntent/11a5ba96-d296-4bb1-b79b-f70004f1deb4/

https://cloud.google.com/dialogflow/es/docs/intents-responses

https://www.geeksforgeeks.org/create-your-own-intents-and-entities-in-dialogflow-chatbot/

https://cloud.google.com/dialogflow/es/docs/intents-actions-parameters

https://botium-docs.readthedocs.io/en/latest/04_usage/index.html#scripting-uttexpansion-incomprehension

https://www.npmjs.com/package/mochawesome

Note: Botium does a static analysis of your conversation flow. The Dialogflow Agent won’t be activated during this analysis, no fulfillment action or anything else will happen. The generated convo files should be seen as starting point for manually refining your test cases.


Testing NLP model of a chatbot:

https://support.botium.ai/hc/en-us/articles/4973861005071-How-to-do-NLU-NLP-Testing-with-Botium-Coach -> The Botium Coach Dashboard visualizes the NLP performance metrics and suggests steps for improving it. It will show any pieces of test data that either did not return the expected intent, did return the expected intent but with a low confidence score, or did return the expected intent, but with a confidence score close to another intent’s.

Rasa is an open source machine learning framework for building AI assistants and chatbots. Mostly you don't need any programming language experience to work in Rasa.

Ref: https://floriantreml.medium.com/tutorial-benchmark-your-chatbot-on-watson-dialogflow-wit-ai-and-more-92885b4fbd48

https://livablesoftware.com/wp-content/uploads/2021/03/TestingNLPBots-BotSE.pdf

https://floriantreml.medium.com/video-tutorial-improve-chatbot-understanding-with-botium-coach-d6882177fc2

Botium coach:

https://support.botium.ai/hc/en-us/articles/4973816377871-Botium-Connectors
https://floriantreml.medium.com/video-tutorial-improve-chatbot-understanding-with-botium-coach-d6882177fc2
https://support.botium.ai/hc/en-us/articles/4973808686095-Step-1-Connect-Botium-Coach-to-Your-Conversational-AI
https://support.botium.ai/hc/en-us/articles/4973827508367-Botium-Coach-NLP-Analytics-Support
