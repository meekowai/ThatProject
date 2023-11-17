Added 'basic-auth'
  - run 'npm install basic-auth' in console
  - declare 'user' and 'secret' in auth.js

    
Added trusted cert for own CA or self-signed cert
  - CameraWeb.ino lines 12-39 and 109

    
If you want to run custom port you need to change it in 3 files:
  - server.js   -> const HTTPS_PORT = PORT;
  - client.html -> const WS_URL = 'wss://' + window.location.hostname + ":PORT";
  - CameraWeb.ino -> const char* websocket_server_host = "wss://192.168.1.80:443";
