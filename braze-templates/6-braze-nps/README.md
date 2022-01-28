# Instructions

Replace the following variables to customize your NPS Survey:

| variable         | description                                                                             | required? |
| ---------------- | --------------------------------------------------------------------------------------- | --------- |
| `SURVEY_ID`      | This ID will be used to log a custom event and custom attribute upon survey submission. | Yes       |
| `QUANT_QUESTION` | The initial question presented in the survey.                                           | Yes       |
| `QUAL_QUESTION`  | The followup question presented with a feedback textarea.                               | No        |
| `AVATAR_IMAGE`   | An optional image to display on top of the survey.                                      | No        |
| `THANKYOU_TEXT`  | The "Thank You" message displayed after completing the survey.                          | No        |
| `SUBHEADER_TEXT` | An optional smaller text to display underneath the initial question.                    | No        |
| `CHOICES`        | An ordered list of choice names. You can remove choices for fewer options.              | No        |

# Data Collection

## Survey Submission

This NPS survey will log a Custom Event (`survey.completed`) when a user submits the survey, or closes the survey after selecting a choice. This event will also include the following properties: 

* `score` - the selected choice number (i.e. 1 through 5)
* `feedback` - the free-form response
* `survey_id` the `SURVEY_ID` configured for this survey
* `url` - the full URL of the current page.

The following Custom Attributes will also be set upon survey submission:

* `survey.${survey_id}.score` - the latest score this user has selected for this survey ID.
* `survey.${survey_id}.feedback` - the latest feedback this user has selected for this survey ID.

Lastly, a "button click" will be recorded using the choice's text, in order to analyze within the message's engagement results in the Braze dashboard.

# Demo

<img alt="screenshot" src="screenshot.gif" height="500"/>
