# Sus Tracker

An Among Us companion that runs in the browser.

- **Crewmate:** log who you saw and where, mark players sus or safe, and check whether it's safe to skip a vote.
- **Impostor:** plan a believable fake-task route, including the second half of two-part tasks like Download/Upload, with a timer for each stop.
- **Voice log:** say "black in admin" and it logs itself. Tap the mic button once and it keeps listening.
- **Your tasks:** say "did swipe card" or "uploaded in admin" to check tasks off, and "what did I do" to hear the list. In meetings, the What you did card shows each one with its room.
- **New game:** say "new game", or "new game, I'm impostor", to start fresh with the same lobby.

The whole app is one file, `index.html`, with no build step. Vercel serves it as a static site.

Hands-free listening needs the page on its own `https://` address, because browsers only let a page use the microphone there. The speech-to-text comes from the browser itself (Chrome sends the audio to Google to turn it into text).
