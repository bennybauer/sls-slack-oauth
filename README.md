# sls-slack-oauth
[![](https://travis-ci.org/bennybauer/sls-slack-oauth.svg?branch=master)](https://travis-ci.org/bennybauer/sls-slack-oauth)

[Serverless Framework](https://github.com/serverless/serverless) function for Slack applications authorization.

Can be used by Serverless Framework projects to handle Slack application authorization boilerplating.

## Usage
In your Serverless Framework project:

    sls function create functions/slack-oauth
        
Copy this repo into your Serverless Framework project.

Change `s-variables-common.json.template` to `s-variables-common.json` and fill it with the required settings.

If needed, tweak `functions/slack-oauth/s-function.js` to adhere to your desired redirect_uri endpoint.

Create the dependencies packages:

    pip install -t functions/vendored/ -r requirements.txt

Deploy it!

    sls dash deploy
