---
Title: "Chatbot answers"
---

??? note "Work in progress"
    - Azure bot [cards](https://docs.microsoft.com/en-us/azure/bot-service/bot-service-design-user-experience?view=azure-bot-service-4.0#cards)


# Chatbot answers :fontawesome-solid-robot:{: .grey }

## Overview

Chatbot questions will be responded to by providing:

1. the answer, e.g. "*Alex Bailey* is responsible for the application *Dynamics 365*"
1. a clarifying question, e.g. "Do you mean *Dynamics 365 Marketing* or *Dynamics 365 Field Service*?" 
1. how to access the answer, if the answer cannot be displayed in the chatbot response, e.g. "To see a list of all Applications and who is responsible, view the [Inventory][inventory]."
1. the Chatbots inability to answer the question and a call to action, e.g. "I'm sorry I don't understand. I can answer these [questions](../chatbot/#user-groups)."
1. a small talk reply and call to action  e.g. "My name is Ita. How can I help?."

The format of answers and the ability to show multiple factsheet cards will depend on the Chat platform used, e.g. Slack, [Teams](https://docs.microsoft.com/en-us/microsoftteams/platform/bots/what-are-bots), 

## Answers

#### An answer about the collection of factsheets

The Chatbot can provide an answer about a collection of factsheets and one or more factsheet cards. These cards can be clicked to open the factsheet in the LeaniX inventory.

![Chatbot Answer](../assets/images/chatbot-answer.png)

*Chatbot's answer to "How many applications do we have?", with extra information about recently created applications.*

#### An answer returning multiple factsheets

![Chatbot Answer](../assets/images/chatbot-multiple-answers.png)

*Chatbot provides a set of factsheets when asked, "Which application supports process Corporate Communications?".*

#### A sample factsheet card 

It may be useful to style factsheet cards based on the cards shown within LeaniX:

![Chatbot Factsheet Card](../assets/images/chatbot-card-application.png)

*Factsheet card from LeanIX.*

## Clarifying question

Ask to choose between two or more factsheet cards to clarify the question:

![Chatbot Answer](../assets/images/chatbot-clarification.png)

*Chatbot seeks clarification about which "Intranet" application when asked, "Who is responsible for application Intranet?".*

## How to access the answer

Show a link to a report in the LeanIX Report Gallery.

## Apology

Apologise for not being to answer and explain what [questions you can answer](../chatbot/#user-groups).  

## Small talk 

Respond to small talk and explain what [questions you can answer](../chatbot/#user-groups).    
