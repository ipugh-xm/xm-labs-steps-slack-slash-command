# Slack Slash Command Steps

This step parses the HTTP POST request made by a slack slash command.


---------

<kbd>
  <img src="https://github.com/xmatters/xMatters-Labs/raw/master/media/disclaimer.png">
</kbd>

---------

# Files

* [SlackSlashCommandSteps.zip](SlackSlashCommandSteps.zip) - Workflow zip file with the step and example flow
* [Slack.png](/Slack.png) - Slack logo

# How it works
Accepts a post request, then gives back the user_name, user_id, command, channel_name, channel_id, and text parameters.


# Installation

## Slack Setup
Requires a custom slack [app](https://api.slack.com). Within a slash command in the app, set the Request URL as the initiation URL from xMatters.

## xMatters Setup
1. Download the [SlackSlashCommandSteps.zip](SlackSlashCommandSteps.zip) file onto your local computer
2. Navigate to the Developer tab of your xMatters instance
3. Click Import, and select the zip file you just downloaded


## Usage
The **Slack - Parse Slash Command** HTTP Trigger is now available in your custom steps. So navigate to the appropriate canvas so you can add the step there. If you'd like to experiment with it, the **Slack Slash Command** workflow has a canvas that can be triggered via HTTP call. 


### Outputs

| Name | Description |
| ---- | ----------  |
| user_name | Username of slash command caller |
| user_id | user_id of slash command caller |
| command | Slash command that was called |
| channel_name | Name of channel where slash command was called |
| channel_id | ID of channel where slash command was called |
| text | Text that was put after the slash command |


## Example
This is an example of using the **Slack - Parse Slash Command** to trigger an xMatters event.

<kbd>
	<img src="/media/ExampleFlow.png">
</kbd>

