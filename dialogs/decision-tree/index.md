# Decision Tree Dialogs

Decision Tree Dialogs are made up of [Utterances](../utterances), [Routes](../routes), and [Actions](../actions).

Nodes

The follow a specific algorithm:

* Is this a new conversation?

    * If yes, initialize a new [Conversation State](../../conversations), send the Utterance(s) associated with the root Dialog Node to this user, and wait for their response

    * If no, retrieve the Conversation State so that it can pick up from where it left off

    * Compare the user's response to the Routes associated with the current Dialog Node.  When a Route matches (i.e. deemed applicable for handling the response), follow it.

    * In following a Route, there are several response options: Sub-Dialogs, Transfer, Terminate, and going on to a specific Dialog Node (which could be the current node if the Bot needs to repeat itself)
