# cloudflare-cors-anywhere
Cloudflare CORS proxy in a worker.

CLOUDFLARE-CORS-ANYWHERE

Source:
https://github.com/Zibri/cloudflare-cors-anywhere

Demo:
https://test.cors.workers.dev

Post:
http://www.zibri.org/2019/07/your-own-cors-anywhere-proxy-on.html

Example:
```javascript
fetch('https://test.cors.workers.dev/?https://httpbin.org/post', {
  method: 'post',
  headers: { 'x-foo': 'bar', 'x-cors-headers': 'aditional headers' }
}).then(r => r.json()).then(console.log)
```

Note:
All received headers are also returned in "cors-received-headers" header.
