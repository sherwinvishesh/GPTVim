# GPTVim

## Overview
GPTVim is a revolutionary plugin designed for Vim and NVim editors, integrating the capabilities of OpenAI's GPT (currently gpt3.5-turbo-16k) directly into your development environment. This tool aims to enhance your coding and development workflow by providing instant, context-aware assistance directly within your editor. Whether you need coding advice, documentation lookups, or just want to chat with GPT, GPTVim brings the power of advanced AI models to your fingertips.

## Features
- **GPT Integration**: Chat with GPT in a separate buffer, with output presented in markdown for clarity.
- **Session Memory**: GPT can recall the context from the current session, ensuring continuity in your interactions.
- **Code Execution**: Execute Python and Lua code snippets and interact directly with your editor, enhancing your coding efficiency.
- **Web Search**: Perform web searches (Google, DuckDuckGo, Wikipedia) and read web page contents without leaving your editor.
- **Text/Code Selection**: Easily append selected text or code to the prompt for context-aware responses.
- **Language Awareness**: The plugin recognizes the language of your current buffer, tailoring GPT's responses accordingly.
- **Multiple Sessions**: Save and continue conversations across multiple sessions, preserving context and progress.

## User Interface

https://github.com/sherwinvishesh/GPTVim/assets/60791187/fda2bb9d-3446-4bb7-b38c-327c0db9499e

## Requirements
To utilize GPTVim, install the github repository and ensure you have the necessary dependencies installed. Use the following command to install the required Python packages:
```bash
git clone https://github.com/sherwinvishesh/GPTVim.git
cd GPTVim
pip3 install -r requirements.txt
```

## Installation
Integrate GPTVim into your development setup through a simple installation process:
```vim
Plug '<user>/GPTVim'
```

## Commands
GPTVim introduces a set of commands to streamline your interaction with GPT:
```
:call gpt#Assist(0)<cr>      # Launch GPT prompt
:'<,'>call gpt#Assist(1)<cr> # Append selection and launch GPT prompt
:call gpt#List()<cr>         # List and manage saved conversations
```

## Key Mappings
Configure default key mappings to quickly access GPTVim features, customizable in your .vimrc file:
```
nmap <silent> gpa <Plug>(GPTVim-assist)
xmap <silent> gpa <Plug>(GPTVim-assist-vis)
vmap <silent> gpa <Plug>(GPTVim-assist-vis)
nmap <silent> gpl <Plug>(GPTVim-conversations)
```

## GPT Buffer Keys
Navigate and manage the GPT buffer with these keys:
- `r`: Reset current session (clears memory and buffer).
- `q`: Close GPT buffer (memory is retained for future recall).
- `s`: Save current session history.
- `L`: List and manage saved sessions.
- `c`: Cancel the current stream (the pending response is discarded).
- `B`: Enter Block Mode for advanced code manipulation.

## Block Mode Commands
In Block Mode, use these commands for efficient code block management:
- `j`: Move to the next code block.
- `k`: Move to the previous code block.
- `y`: Copy the current code block and exit Block Mode.

## Session Management
Effortlessly manage your saved sessions with these keys:
- `q`: Close the session list.
- `d`: Delete the selected session.
- `<cr>`: Load the selected session.
- `s`: Open the selected conversation in a horizontal split.
- `v`: Open the selected conversation in a vertical split.

## Contributing

Contributions to enhance this project are welcomed. Please feel free to fork the repository, make changes, and submit pull requests.

## Support

If you encounter any issues or have any questions, please submit an issue on the GitHub issue tracker or feel free to contact me.


## License

GPTVim is open source and available under the [Apache-2.0 license](LICENSE).

## Acknowledgments


- Thanks to everyone who visits and uses this page. Your interest and feedback are what keep us motivated.
- Special acknowledgment to kampu for his recommendations. It served as a significant inspiration for this project, demonstrating the powerful impact of generative ai in a text editor.

## Connect with Me

Feel free to reach out and connect with me on [LinkedIn](https://www.linkedin.com/in/sherwinvishesh) or [Instagram](https://www.instagram.com/sherwinvishesh/).

---

Made with ❤️ by Sherwin
