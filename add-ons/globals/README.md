# Globals Add-on

With this Configuration active, you can set global settings for your Bot which can be referenced dynamically in conversation.

For example, if you want your Bot to respond with a phone number, but you'd like the option of updating that phone number in the future without having to edit multiple Dialogs which respond with that phone number, setting a Global variable is a good option.  To do this, create a Global value called `phone_number` and set it to something like 800-555-1212.  Then, when you are writing Utterances for your Bot, you can reference this value in the following way:

> You can reach me at `{bot.phone_number}` on weekdays from 9am-5pm PST.

The phone number you set will be dynamically populated when this response is sent to the user.  You can update this value at any time on the Globals tab of your Bot.
