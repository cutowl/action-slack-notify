# action-slack-notify

Action to notify slack channel about workflow status, based on rtCamp action (rtCamp/action-slack-notify)

## Usage Example
```yaml
post_action_job:
    runs-on: ubuntu-latest
    steps:
      - name: Slack Notify
        uses: cutowl/action-slack-notify@v0.0.2
        env:
          ENVIRONMENT: production
          SLACK_CHANNEL: test-deploy
          SLACK_COLOR: success
          SLACK_FOOTER: 'footer text'
          SLACK_TOKEN: ${{ secrets.SLACK_TOKEN }}
      
```