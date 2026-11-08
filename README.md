# Sus Tracker

An Among Us companion that runs in the browser.

- **Crewmate:** log who you saw and where, mark players sus or safe, and check whether it's safe to skip a vote.
- **Impostor:** plan a believable fake-task route, including the second half of two-part tasks like Download/Upload, with a timer for each stop.
- **Voice log:** say "black in admin" and it logs itself. Tap the mic button once and it keeps listening.
- **Your task list:** read it off the game screen once, like "my tasks are admin swipe card, cafeteria download, electrical wires". As an impostor that becomes your fake route, and "done" walks it stop by stop. As a crewmate it's your checklist.
- **Checking tasks off:** say "did download" or "did swipe card". The room comes from your list, so you never say where you are. "What did I do" shows the list, and in meetings the What you did card shows each task with its room.
- **Task board:** the top of the Tasks tab fits your whole list on one screen. Tap a circle to check a task off, tap again to uncheck it, and × takes it off your list. As an impostor the next stop sits on top with a Done button.
- **New game:** say "new game", or "new game, I'm impostor", to start fresh with the same lobby.
- **Lobby:** "add black", "remove color black", "add cyan and lime". "Remove swipe card" takes a task off your list.

The whole app is one file, `index.html`, with no build step. Vercel serves it as a static site.

Hands-free listening needs the page on its own `https://` address, because browsers only let a page use the microphone there. The speech-to-text comes from the browser itself (Chrome sends the audio to Google to turn it into text).
