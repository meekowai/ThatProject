Added 'basic-auth'
  - run 'npm install basic-auth' in console
  - declare 'user' and 'secret' in auth.js

If you want to run custom port you need to change it in two files:
  - server.js   -> const HTTPS_PORT = PORT;
  - client.html -> const WS_URL = 'wss://' + window.location.hostname + ":PORT";
