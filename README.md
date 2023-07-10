# [Chat Chat](https://chat.okisdev.com)

> Chat Chat to unlock your next level AI conversational experience. You can use multiple APIs from OpenAI, Microsoft Azure, Claude, Cohere, Hugging Face, and more to make your AI conversation experience even richer.

[![LICENSE](https://img.shields.io/github/license/okisdev/ChatChat?style=flat-square)](https://github.com/okisdev/ChatChat/blob/master/LICENSE) [![Twitter](https://img.shields.io/twitter/follow/okisdev)](https://twitter.com/okisdev) [![Telegram](https://img.shields.io/badge/Telegram-Chat%20Chat-blue?style=flat-square&logo=telegram)](https://t.me/+uWx9qtafv-BiNGVk)

<p align='center'>
    <a>English</a> | <a href='README.zh_HK.md'>繁体中文</a> | <a href='README.zh_CN.md'>简体中文</a> | <a href='README.JA.md'>日本語</a>
</p>

<p align='center'>
    <a href='https://docs.okis.dev/chat' target='_blank'>
        Documentation
    </a>
    | <a href='https://github.com/okisdev/ChatChat/issues/3'>Common Issue</a>
</p>

## Important Notes

-   Some APIs are paid APIs, please make sure you have read and agreed to the relevant terms of service before use.
-   Some features are still under development, please submit PR or Issue.
-   The demo is for demonstration purposes only, it may retain some user data.
-   AI may generate offensive content, please use it with caution.

## Preview

### Interface

![UI](https://cdn.harrly.com/project/GitHub/Chat-Chat/img/UI-1.png)

![Dashboard](https://cdn.harrly.com/project/GitHub/Chat-Chat/img/Dashboard-1.png)

### Functions

https://user-images.githubusercontent.com/66008528/235539101-562afbc8-cb62-41cc-84d9-1ea8ed83d435.mp4

https://user-images.githubusercontent.com/66008528/235539163-35f7ee91-e357-453a-ae8b-998018e003a7.mp4

## Features

-   [x] TTS
-   [x] Dark Mode
-   [x] Chat with files
-   [x] Markdown formatting
-   [x] Multi-language support
-   [x] Support for System Prompt
-   [x] Shortcut menu (command + k)
-   [x] Wrapped API (no more proxies)
-   [x] Support for sharing conversations
-   [x] Chat history (local and cloud sync)
-   [x] Support for streaming messages (SSE)
-   [x] Plugin support (`/search`, `/fetch`)
-   [x] Support for message code syntax highlighting
-   [x] Support for OpenAI, Microsoft Azure, Claude, Cohere, Hugging Face

## Roadmap

Please refer to https://github.com/users/okisdev/projects/7

## Usage

### Prerequisites

-   Any API key from OpenAI, Microsoft Azure, Claude, Cohere, Hugging Face

### Environment variables

| variable name     | description                 | default | mandatory | prompt                                                                                                            |
| ----------------- | --------------------------- | ------- | --------- | ----------------------------------------------------------------------------------------------------------------- |
| `DATABASE_URL`    | Postgresql database address |         | **Yes**   | Start with `postgresql://` (if not required, please fill in `postgresql://user:password@example.com:port/dbname`) |
| `NEXTAUTH_URL`    | Your website URL            |         | **Yes**   | (with prefix)                                                                                                     |
| `NEXTAUTH_SECRET` | NextAuth Secret             |         | **Yes**   | Random hash (16 bits is best)                                                                                     |
| `EMAIL_HOST`      | SMTP Host                   |         | No        |                                                                                                                   |
| `EMAIL_PORT`      | SMTP Port                   |         | No        |                                                                                                                   |
| `EMAIL_USERNAME`  | SMTP username               |         | No        |                                                                                                                   |
| `EMAIL_PASSWORD`  | SMTP password               |         | No        |                                                                                                                   |
| `EMAIL_FORM`      | SMTP sending address        |         | No        |                                                                                                                   |

### Deployment

> Please modify the environment variables before deployment, more details can be found in the [documentation](https://docs.okis.dev/chat/deployment/).

#### Local Deployment

```bash
git clone https://github.com/okisdev/ChatChat.git
cd ChatChat
cp .env.example .env
yarn
yarn dev
```

#### Vercel

[![Deployed in Vercel](https://vercel.com/button)](https://vercel.com/import/project?template=https://github.com/okisdev/ChatChat)

#### Zeabur

Visit [Zeabur](https://zeabur.com) to deploy

#### Railway

[![Deploy on Railway](https://railway.app/button.svg)](https://railway.app/template/-WWW5r)

#### Docker

```bash
docker build -t chatchat .
docker run -p 3000:3000 chatchat -e DATABASE_URL="" -e NEXTAUTH_URL="" -e NEXTAUTH_SECRET="" -e EMAIL_HOST="" -e EMAIL_PORT="" -e EMAIL_USERNAME="" -e EMAIL_PASSWORD="" -e EMAIL_FORM=""
```

OR

```bash
docker run -p 3000:3000 -e DATABASE_URL="" -e NEXTAUTH_URL="" -e NEXTAUTH_SECRET="" -e EMAIL_HOST="" -e EMAIL_PORT="" -e EMAIL_USERNAME="" -e EMAIL_PASSWORD="" -e EMAIL_FORM="" ghcr.io/okisdev/chatchat:latest
```

## LICENSE

[AGPL-3.0](./LICENSE)

## Support me

[![Buy Me A Coffee](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/okisdev)

## Technology Stack

nextjs / tailwindcss / shadcn UI
