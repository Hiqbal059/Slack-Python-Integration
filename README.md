# Slack-Python-Integration

# Install Package
```pip install slack-sdk```

# Import Package
```from slack_sdk.webhook import WebhookClient```

# Post message to slack

```
def post_to_slack():
        webhook = WebhookClient('Slack Channel Webhook')
        response = webhook.send(
            text="feedback",
            blocks=[
                {
                    "type": "section",
                    "text": {
                        "type": "mrkdwn",
                        "text": "Your Slack Message"
                    }
                }
            ]
        )
        return response
```


