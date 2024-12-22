# MultiAgent ChatLab

A browser-based interface for experimenting with multi-agent conversations using various LLM APIs. Have conversations between different AI models or observe how they interact with each other - all directly in your browser. For more information check out [this piece](https://benjamintseng.com/portfolio/multi-agent-chatlab/)

## Features

- Pure client-side implementation - no server required
- Support for multiple LLM providers:
  - Google (Gemini models)
  - Anthropic (Claude models)
  - OpenAI models
- Real-time conversation history including Markdown rendering support (via [Showdown](https://github.com/showdownjs/showdown)) and color-coded messages for easy agent tracking
- Editable message history to facilitate experimentation
- Simple tabbed interface supports up to 6 agents (each can have own system prompts and models)

## Quick Start

1. Clone this repository or just download `multiagent-chatlab.html`
2. Open `multiagent-chatlab.html` in your browser
3. Configure the agents (with your own LLM API keys, names, and system prompts)
4. Start chatting!

## Security Note

This tool runs entirely in your browser. Your API keys are never sent anywhere except directly to the respective LLM providers' APIs. However, always use API keys responsibly.

## How It Works

The ChatLab allows you to:
1. Customize Agents (you can pick model, name, and system prompt)
2. Send messages as a user or pick Agent to respond next in a conversation
3. Edit or delete any message in the conversation history

Each message in the conversation is color-coded by sender for easy tracking of who said what (for up to 6 total participants). The interface automatically handles the appropriate API formatting for each provider's chat history requirements and does simple prefix adding / removing behind-the-scenes.

## Requirements

- A modern web browser
- API key(s) for the LLM provider(s) you want to use:
  - [Google AI API key](https://ai.google.dev/gemini-api/docs/api-key) for Gemini models
  - [Anthropic API key](https://docs.anthropic.com/en/api/getting-started) for Claude models
  - [OpenAI API key](https://platform.openai.com/docs/api-reference/introduction) for OpenAI models

## Development

This project is built using:
- [Preact](https://preactjs.com/) for UI components
- [htm](https://github.com/developit/htm) for JSX-like syntax without build steps
- [Showdown](https://github.com/showdownjs/showdown) for in-browser Markdown rendering
- Pure browser JavaScript - no bundler or build process required

## Contributing

Some areas that could use improvement:
- Additional LLM provider support
- Improved error handling
- More customization options for system prompts
- Conversation templates/presets

## License

MIT License

## Credits

Created by [Benjamin Tseng](https://benjamintseng.com/)