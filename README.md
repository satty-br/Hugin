# Hugin
### Hugin is a project that validates the secrets found by gitleaks, a tool that detects leaked credentials in git repositories.


### put the project folder in the same directory or set the variable --project

Installation
Clone the project repository to your local machine
Install the project dependencies with the command:
````
pip install -r requirements.txt
````
Usage

Run the main.py file with the gitleaks results file in JSON format as an argument and set the project folder because I need to search for information within the files:

````
python main.py --project ./project ./results.json
````

Hugin will read the JSON file and show the details of the secrets on the screen

Hugin will also return a new file output.json with the same format as the gitleaks file, but with an additional property called valid, which can be true or false
If valid is true, it means that Hugin validated the secret and confirmed that it is a valid credential
If valid is false, it means that the secret can be an invalid credential or a false positive, in that case, you need to do a double check

## keys
- [ ] adafruit-api-key
- [ ] adobe-client-id
- [ ] adobe-client-secret
- [ ] age secret key
- [ ] airtable-api-key
- [ ] algolia-api-key
- [ ] alibaba-access-key-id
- [ ] alibaba-secret-key
- [ ] asana-client-id
- [ ] asana-client-secret
- [ ] atlassian-api-token
- [ ] authress-service-client-access-key
- [X] aws-access-token
- [ ] beamer-api-token
- [ ] bitbucket-client-id
- [ ] bitbucket-client-secret
- [ ] bittrex-access-key
- [ ] bittrex-secret-key
- [ ] clojars-api-token
- [ ] codecov-access-token
- [ ] coinbase-access-token
- [ ] confluent-access-token
- [ ] confluent-secret-key
- [ ] contentful-delivery-api-token
- [ ] databricks-api-token
- [ ] datadog-access-token
- [ ] defined-networking-api-token
- [ ] digitalocean-access-token
- [ ] digitalocean-pat
- [ ] digitalocean-refresh-token
- [ ] discord-api-token
- [ ] discord-client-id
- [ ] discord-client-secret
- [ ] doppler-api-token
- [X] droneci-access-token
- [ ] dropbox-api-token
- [ ] dropbox-long-lived-api-token
- [ ] dropbox-short-lived-api-token
- [ ] duffel-api-token
- [ ] dynatrace-api-token
- [X] easypost-api-token
- [X] easypost-test-api-token
- [ ] etsy-access-token
- [ ] facebook
- [ ] fastly-api-token
- [ ] finicity-api-token
- [ ] finicity-client-secret
- [ ] finnhub-access-token
- [ ] flickr-access-token
- [ ] flutterwave-encryption-key
- [ ] flutterwave-public-key
- [ ] flutterwave-secret-key
- [ ] frameio-api-token
- [ ] freshbooks-access-token
- [X] gcp-api-key
- [ ] generic-api-key
- [X] github-app-token
- [X] github-fine-grained-pat
- [X] github-oauth
- [X] github-pat
- [X] github-refresh-token
- [X] gitlab-pat
- [X] gitlab-ptt
- [X] gitlab-rrt
- [ ] gitter-access-token
- [ ] gocardless-api-token
- [X] grafana-api-key
- [ ] grafana-cloud-api-token
- [X] grafana-service-account-token
- [ ] hashicorp-tf-api-token
- [X] hashicorp-tf-password
- [X] heroku-api-key
- [ ] hubspot-api-key
- [ ] huggingface-access-token
- [ ] huggingface-organization-api-token
- [ ] infracost-api-token
- [ ] intercom-api-key
- [X] jfrog-api-key
- [X] jfrog-identity-token
- [ ] jwt
- [ ] jwt-base64
- [ ] kraken-access-token
- [ ] kucoin-access-token
- [ ] kucoin-secret-key
- [ ] launchdarkly-access-token
- [ ] linear-api-key
- [ ] linear-client-secret
- [ ] linkedin-client-id
- [ ] linkedin-client-secret
- [ ] lob-api-key
- [ ] lob-pub-api-key
- [ ] mailchimp-api-key
- [ ] mailgun-private-api-token
- [ ] mailgun-pub-key
- [ ] mailgun-signing-key
- [ ] mapbox-api-token
- [ ] mattermost-access-token
- [ ] messagebird-api-token
- [ ] messagebird-client-id
- [ ] microsoft-teams-webhook
- [ ] netlify-access-token
- [ ] new-relic-browser-api-token
- [ ] new-relic-user-api-id
- [ ] new-relic-user-api-key
- [ ] npm-access-token
- [ ] nytimes-access-token
- [ ] okta-access-token
- [ ] openai-api-key
- [ ] plaid-api-token
- [ ] plaid-client-id
- [ ] plaid-secret-key
- [ ] planetscale-api-token
- [ ] planetscale-oauth-token
- [ ] planetscale-password
- [ ] postman-api-token
- [ ] prefect-api-token
- [ ] private-key
- [ ] pulumi-api-token
- [ ] pypi-upload-token
- [ ] rapidapi-access-token
- [ ] readme-api-token
- [ ] rubygems-api-token
- [ ] scalingo-api-token
- [ ] sendbird-access-id
- [ ] sendbird-access-token
- [ ] sendgrid-api-token
- [ ] sendinblue-api-token
- [ ] sentry-access-token
- [ ] shippo-api-token
- [ ] shopify-access-token
- [ ] shopify-custom-access-token
- [ ] shopify-private-app-access-token
- [ ] shopify-shared-secret
- [ ] sidekiq-secret
- [ ] sidekiq-sensitive-url
- [ ] slack-app-token
- [ ] slack-bot-token
- [ ] slack-config-access-token
- [ ] slack-config-refresh-token
- [ ] slack-legacy-bot-token
- [ ] slack-legacy-token
- [ ] slack-legacy-workspace-token
- [X] slack-user-token
- [ ] slack-webhook-url
- [ ] snyk-api-token
- [ ] square-access-token
- [ ] squarespace-access-token
- [ ] stripe-access-token
- [ ] sumologic-access-id
- [ ] sumologic-access-token
- [ ] telegram-bot-api-token
- [ ] travisci-access-token
- [ ] twilio-api-key
- [ ] twitch-api-token
- [ ] twitter-access-secret
- [ ] twitter-access-token
- [ ] twitter-api-key
- [ ] twitter-api-secret
- [ ] twitter-bearer-token
- [ ] typeform-api-token
- [ ] vault-batch-token
- [ ] vault-service-token
- [X] yandex-access-token
- [X] yandex-api-key
- [X] yandex-aws-access-token
- [X] zendesk-secret-key