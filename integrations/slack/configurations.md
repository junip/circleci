# Slack Integrations 

## [Setup Slack APP](https://github.com/CircleCI-Public/slack-orb/wiki/Setup)

- [create slack app ](https://api.slack.com/apps)
- Permissions - setup permission the app
- install and receive tokens/
- install app to your workspace.
- Add a default slack channel so that if not `channelid` is specified then it will push notification to the default workspace.
- Get the channel Id by opening the slack in broswer 
  `url/channelID` - channel id starts with `C`

- After above changes add the notification configurations in config.yml


## Config file Changes.
- you have to first add the orb to get the slack notifications
```
slack: circleci/slack@4.4.0
```

- Then in the `config.yml` file add the following changes to `config` ( in your build process)

```
- slack/notify:
  # notify slack if the job fails
  event: fail
  template: basic_fail_1
  channel: <your slack channel Id>
```


## Slack Orb Available template

- `basic_success_1`
  - Should be used with the "pass" event.
- `basic_fail_1`	
  - Should be used with the "fail" event.
- `success_tagged_deploy_1`	
  - To be used in the event of a successful deployment job.
- `basic_on_hold_1`  
  - To be used in the on-hold job.( where you are required to approve build which are in hold)