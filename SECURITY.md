# Security policy

## Reporting a vulnerability

Please **don't open a public issue** for security problems.

Report it privately through GitHub: go to the **Security** tab of this repository and
click **Report a vulnerability**. Include what you found, how to reproduce it, and what
someone could do with it.

You'll get an answer as soon as possible. This is a small volunteer project, so please
allow a few days.

## Scope

Today the repository only has documentation and a static prototype with sample data.
Nothing is stored and there are no accounts. Once the app has a backend, this file will
list what's in scope.

## Never commit secrets

API keys and other secrets go in a local `.env` file, which is ignored by Git. Secret
scanning and push protection are enabled on this repository.
