# Conversations

When any User interacts with the same Bot, we call this a **Conversation**.

Try cloning the [Favorite Foods](../bots/templates/favorite-foods) bot for a simple example use case.


### Usage: Reference a system value

TODO: gif animation of creating Utterance and seeing Rendered response

## Global State

The [Global State](../add-on/global-state) add-on provides a special memory for Bots.  A Bot's author can manually enter data into the Global State and reference.

### Usage: Reference a global value

TODO: gif animation of creatting Utterance and seeing Rendered response


## Conversation State

When a Bot first encounters a new user, it creates a record in it's memory and initializes it will some basic details it can gather about the user.  The Conversation State can be updated...

* by the Bot to store system information
* when an [Action](../actions) is executed
* if an [Add-on](../add-ons) is configured to do so

In contrast to the Global State, the Conversation State is specific to each user, and the Bot has no ability to leverage information from one private Conversation in another.  Only the Global State is common.

Frequently, various [Dialogs](../dialogs), [Routes](../routes), and [Actions](../actions) will store useful bits of information for you.

## Data Types

Any datum stored in the Bot's state is called an Attribute.  Attributes can take on many forms, but the most common is a key/value pair.  The `Add Attribute` Action is a popular way to add details to the conversation state, but there are many other ways.

In general, data from the Conversation State or Global State is "flexibly typed".  In many programming languages, one must carefully consider the "type" o the variable (e.g. text, number, etc).  Bots store information in a generic way and will try to use the value in whatever type is more appropriate for the situation, be is a number, date/time, phone number, or general text.

TODO: screenshot of a conversation state

TODO: explain the namespace and format {user.no_spaces_or_caps}

### Attribute Sets

As the name implies, Attribute Sets are a special type of Attribute in which the Bot can maintain a collection of items that belong together and update that in the ways one would update a typical set (adding and removing items), typically using [Actions](../actions), such as `Add to Set`, `Remove from Set`, and `Clear a Set`.



