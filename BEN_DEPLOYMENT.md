# Personal quick deployment on self-hosted server

- git clone https://github.com/BenjaminPiette/chat-with-gpt.git
- cd chat-with-gpt/app
- npm i -D
- npm run build
- npm install -g http-server
- ufw allow 4545
- npm i -g forever
- forever start $(which http-server) -p 4545 -d false
- forever list