# skipset-sms

Static `sms:` redirect page used by the Skipset Telegram bot.

Telegram strips `sms:` from links and URL buttons, so the lead-alert "Message as
Investor/Realtor" buttons can't deep-link into Messages directly. This page takes
`?to=+1…&b=<message>` and bounces the browser to `sms:+1…&body=<message>`, which
opens iMessage/SMS pre-filled on iPhone and Mac.

Served via GitHub Pages: <https://skipset-ai.github.io/skipset-sms/>

Source lives in [`Skipset-AI/skipset.data`](https://github.com/Skipset-AI/skipset.data) at
`mvp/web/index.html`; this repo is just the public host.
