# Thinkjs
learn thinkjs

> Node.js 提供 http 模块直接创建 HTTP 服务, 用来响应用户的请求, 比如 Node.js 官网提供的创建 HTTP 服务的例子:

```JavaScript

const http = require('http')
const hostname = '127.0.0.1'
const port = 3000

const server = http.createServer((req, res) => {
  res.statusCode = 200
  res.setHeader('Content-Type', 'text/plain')
  res.send('Hello World\n')
})

server.listen(port, hostname, () => {
  console.log(`Server running at http://${hostname}:${port}`)
})

```

Thinkjs也是调用 http.createServer 的方式来创建服务的, 因此整个运行流程包含了启动服务和响应用户请求两个部分



