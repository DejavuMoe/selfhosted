## Twikoo

>A simple, safe and free comment system.

- Source Code: https://github.com/twikoojs/twikoo
- Website: https://twikoo.js.org/

### Get Start

- Install Docker and Docker Compose
- A Web Server like Nginx or Caddy

### Install Twikoo

Use the [docker-compose.yml](docker-compose.yml) to as a docker compose template, then

```bash
sudo docker compose up -d
```

### Nginx Reverse Proxy

- Use the [nginx.conf](nginx.conf) as a Nginx VHost template in `/etc/nginx/conf.d/twikoo.your.domain.conf`.
- Modify some of the required information inside, such as your actual domain name, SSL certificate path, log path, etc.
- Then just resolve the domain name to your server IP address, e.g.`twikoo.your.domain` to `131.34.2.9`

Reload Nginx Config:

```bash
sudo nginx -t
sudo nginx -s reload
```

Check the twikoo site in your domain, e.g. `twikoo.your.domain`, if it works well you will see

```json
{
  "code": 100,
  "message": "Twikoo 云函数运行正常，请参考 https://twikoo.js.org/frontend.html 完成前端的配置",
  "version": "1.6.44"
}
```

### Add Twikoo to your site

```html
<div id="tcomment"></div>
<script src="https://cdn.jsdelivr.net/npm/twikoo@1.6.44/dist/twikoo.min.js"></script>
<script>
twikoo.init({
  envId: 'https://twikoo.your.domain', // Replay with your Twikoo domain.
  el: '#tcomment',
  lang: 'en-US'
})
</script>
```

Just Enjoy it!