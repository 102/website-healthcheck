# Website Simple Healthcheck Action

This actions checks your website if it's returning status code 200.

An example of website-healthcheck in a GitHub Action:

```yaml
name: "Check for website health"

on:
  schedule:
    - cron: "*/12 * * * *"

jobs:
  healthcheck:
    runs-on: ubuntu-latest

    steps:
      - name: Ping uuid
        uses: 102/website-healthcheck@v1.0.0
        with:
          web-url: https://uuid-364w.onrender.com/
```
