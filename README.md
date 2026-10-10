# Living World RP Controller

A controller for long-form, character-driven interactive fiction. It's intended to make NPCs behave like people with their own motivations, relationships and lives, rather than existing solely to respond to the player or advance a plot.

**You control your protagonist. The model controls the NPCs, world and consequences.**

The complete controller is in [`SYSTEM_PROMPT.txt`](SYSTEM_PROMPT.txt).

## ChatGPT — quick start

1. Start a new chat and select **GPT-6 with High thinking**, if available.
2. Paste the complete contents of `SYSTEM_PROMPT.txt` into your first message and send it.
3. Describe your setting, characters and starting situation in the next message. Then play normally.

This is the easiest way to experiment. A message in ChatGPT isn't a true system instruction, though, so results can differ from setups that expose a system-prompt field.

## ChatGPT — using a Project

For an ongoing RP, I recommend a dedicated **ChatGPT Project**:

1. Create a Project and choose **Project-only memory** under Project settings → Memory. This keeps context from other chats and projects out of the RP.
2. Add `SYSTEM_PROMPT.txt` to the Project's files/sources.
3. In **Project settings → Instructions**, add something short like:

   > For RP in this project, use `SYSTEM_PROMPT.txt` as the complete writing and world-behaviour controller, not as fictional lore. I write my protagonist; you write the NPCs, world and consequences. Follow the controller throughout the RP.

4. Start a chat in the Project and describe your scenario. For the closest match to my tests, **also paste the full controller into that chat at the start**.

Project files are reference context, not guaranteed substitutes for direct instructions. The full controller is also too long to fit into typical Project instruction fields. Project-only memory is useful for keeping different RPs separate, but it doesn't guarantee perfect recall of every event.

## SillyTavern

- **Chat Completion APIs:** Put the controller in **AI Response Configuration → Prompt Manager → Main Prompt**.
- **Text Completion APIs:** Use **Advanced Formatting → System Prompt**.
- Add your characters and scenario as normal. If you have another preset full of RP-writing rules, test without conflicting instructions first.

## Notes

The original controller was developed on **GPT-5.6 High**, with the update tested on **GPT-6 High** in ChatGPT. Other models and interfaces may behave differently. This is not a deterministic tabletop rules or dice engine.

[Original GPT-5.6 research post](https://www.reddit.com/r/SillyTavernAI/s/nTfkJAropv)
