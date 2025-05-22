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

This website uses the typical ASF layout. The actual website is found on the branch `asf-site`, any changes need to be pushed there.

You can run

```bash
docker compose up build
```

which will create a folder `_site`. This is the content, which needs to be copied after wards to the `asf-site` branch.
If you wish to see a preview for your branch, you can use `asf-staging` to see a copy hosted under: https://stormcrawler.staged.apache.org/

### Build with GitHub actions

The website is automatically build on a push to `main` and any changes are pushed to the `asf-site` branch.
A preview is available via https://stormcrawler.staged.apache.org/ if you go to the GitHub Actions tab and trigger a manual staging deploy action.  