# Getting Started

TODO: add a video

TODO: write quickstart guide

## Definitions

**Bot** - A Chatbot!

**Primary Channel** - The way in which users can interact with your Bot (e.g. Slack, Facebook, your website).

**Add-On** - Bots can select any number of add-ons to enable additional functionality such as connecting to Zendesk and training custom machine learning models on your data.

[Dialog](./dialogs) - A Bot is composed of one or more Dialogs.  Each Dialog handles a specific aspect of conversation.  Dialogs come in different types.  For example the [FAQ Dialog](./dialogs/faq) is an intuitive Dialog that makes a great place to start.  One of the most popular Dialogs is the [Decision Tree Dialog](./dialogs/decision-tree/)

[Utterances](./utterances) - A single message sent from a Bot to its user.  While this is often a short amount of text, there are a variety of other Utterances such as [Single Select](./utterances/single-select) and [Slider](./utterances/slider).

[Actions](./actions/) - A service the Bot can be configured to perform such as [Send Email](./actions/send/email).

**Route** - Routes are tools for a Bot to recognize and understand the responses of users.  Single routes like [Phrase Match](./routes/basic/phrase) are configured to match certain types of responses only.  When a Route matches a message it is configured to recognize, the Bot will follow that Route.  The Route is configured with logic about what to do next (for example, launch into a specific Dialog).  Routes can also include Actions.

[Conversation and Conversation State](./conversations) - The sequence of interactions between a Chatbot and a single user is called a Conversation and is typically thought of as the "logs" of your Bot.  The Conversation State is the most up to date information a Bot has on a user including where they are in the Conversation, what it has learned about the user, and any information you chose to have the Bot capture along the way.

