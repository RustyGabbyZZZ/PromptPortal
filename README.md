# PromptPortal
This is a localy hosted website ui for lmstudio.
The goal of this project is to give access of an lmstudio instance to all local devices through an html page, even the less powerful ones.

To run this project, start a local lmstudio server in power-user or developer mode with 'serve local network' and 'CORS' enabled.
We proceed by downloading the 2 html files and starting a command line at their directory, after that, start a simple python server with:
python -m http.server 8000

And you're done. You can now access the interface with your hosting device as a web address on your local network.
ex:

device ip: 192.168.1.88

server port: 8000

local website: 192.168.1.88:8000

Quirks:

    The ui leaves to be desired, lol, but it works, mostly, so it's fine.
    Not every llm was tested, gpt-oss 20b was the main testing partner, so response should be great, but reasoning output could be iffy.
    Its possible to switch loaded llms, but not their parameters, so make sure they are ajusted beforehand.
    Chat history doesn't save, for now.
