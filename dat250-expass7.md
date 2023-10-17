I have used python as programming language throughout the exercises.

Link to code for the experiments:
https://github.com/ritaborlaug/messaging-systems

I downloaded RabbitMQ using homebrew.

I then installed pika, which went fine. But when I tried to import pika in my python file, the module was not found. When I googled it, I saw that several other people had had the same issue, but none of the answers worked for me. 
The solution I found was to change to a different interpreter, from python3.12.0 to python3.10.1. This resolved the error.

To run the files from the terminal, I just used python3.10 instead of python3 as keyword, and then the files ran as expected. 