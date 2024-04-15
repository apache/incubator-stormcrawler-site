# Apache StormCrawler Website

## How to build?

This website is build using Jekyll. Make sure to have it available locally.
To build and run server locally type 'jekyll serve'. The site can then be accessed at localhost:4000.

### Docker

You can build the website for local testing by running

```bash
docker compose up local
```


## Deployment

This website uses the typical ASF layout. The actual website is found on `asf-site`. Any changes need to be pushed to this branch.
You can run

```bash
docker compose up build
```

which will create a folder `_site`. This is the content, which needs to be copied ofter to the `asf-site` branch.