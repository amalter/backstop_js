# Starter for Backstop JS
You can clone and follow instructions below or start from scratch by following these installation [instructions](https://github.com/garris/BackstopJS/tree/master#installation).

## Setup
### Intall Backstopjs Globally
- Open terminal and run: `npm install -g backstopjs`

### Clone repo into project 
- cd into project and run:
`git clone git@github.com:amalter/backstop_js.git`

### Set up backstop.json
- Update `"viewports"` with all the viewports you want to test

- Update `"scenarios":` with new labels and URL paths to test

### Create Reference
- Before making changes you'll want to create screenshots of your projects current state to test later
- cd into `backstop_js/` directory and run `backstop reference` to add the `backstop_data/` directory which will hold the reference ("before") screenshots of your project in `bitmaps_reference/`

### Create Test
- Create a feature branch in your project and make the changes
- When you are done and ready to test run `backstop test` this will set up a new directory called `bitmaps_test/` in your `backstop_data/` directory and a new browser window will display the test results

### Additional notes
- Backstop seems to only pick up on changes that impact layout shifts. For example, if making a change to border radius it doesn't call out any issues, but if you make changes to padding, margins, text size, etc. It will pick up on the layout shifts.