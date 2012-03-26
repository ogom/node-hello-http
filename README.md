# node-hello-http 

node.js で記述された簡単な HTTP サーバのサンプルです。

## How to use
ポート8080で HTTP のリクエストを待ち受け、アクセスされると 'Hello World' が表示されます。

```js
var http = require('http');

http.createServer(function (request, response) {
  response.writeHead(200, {'Content-Type': 'text/plain'});
  response.end('Hello World');
}).listen(8080);
```