# gpt-3-5-turbo-web

Access OpenAI's GPT-3.5 model in a web page.

Your API key is configured in a server. Password is needed before invoking the API.

TODO: support conversation with history.

## Deploy

```bash
git clone https://github.com/gpt-3-5-turbo-web/gpt-3-5-turbo-web-docker.git
git submodule update --init --recursive
# Specify your `OPENAI_KEY` in docker-compose.yml file. Also pay attention to `CHINA_WORKAROUND` to use a mirror when building the image.
nano docker-compose.yml
docker-compose build
docker-compose pull
docker-compose up -d
```