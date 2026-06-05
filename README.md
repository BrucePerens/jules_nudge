# jules_nudge
Nudge Google Jules, So that it works non-interactively all night!

This is a silly little program to fix an embarassing but long-persistent
Google bug. Jules tends to stop, claiming it has failed, for no
reason. Its system prompt injects a requirement to interact with the
user after your prompt. So, if you want Jules to work on a long task
all night while you sleep, it won't, without this program.

This program works by waking up once a minute and checking the status
of all of your running Jules sessions. When Jules stalls, the program
sends it a message "Proceed". When Jules has a question for the user,
it tells them the user isn't available for input. When Jules wants plan
approval, the program approves.

This is usually enough to keep Jules running until it's done.

Set JULES_API_KEY in the environment, and run the program. Leave it running
while your Jules sessions are working autonomously.
