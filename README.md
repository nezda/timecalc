TimeCalc
========
A simple timesheet calculator for adding up hours worked.  You can see a live version here: http://timecalc.herokuapp.com

I designed this to have a small app to tinker with JavaScript and related technologies. So far it incorporates: 
* [JQuery] for UI behavior
* [Bootstrap] for styling
* [Moment] for time parsing
* [Jasmine] for BDD specification tests
* [Heroku] for hosting using a thin Ruby [Rack] layer

In the future I play to try out:
* [Cucumber] acceptance testing
* [Knockout] for UI interactions
* [Mustache] templating
* [LESS] for CSS
* Underscore or Lo-Dash for functional constructs

Todo
----
- rearrange files in directories
- Github for feedback -- how to allow comments?
- HTML validation
- CSS validation
- JSLint
- solicit feedback
- Switch to using Web Hosted JS files? for jquery?
* tool tips on headers with help
* garbage times should not convert ("kjsdf" or "900")
- should leave break times there, normalized??
* Should allow checkbox to round to nearest .25
* times like "900"

Questions
---------
- better to be more specific or general in selectors?
- how to properly center the h1
- should i have used tables, and nested tables?
- consider using input type=time, number; what versions are supported?

Stories Complete
-----------------
- should display 5 rows with 3 columns
- should label rows: day 1, day 2, ...
- should display 3 column headers: Time In, Time Out, Break Length
- alignment in input fields should be on right side
- after each focus change, should update hours for each day after entered
- after each focus change, should compute total hours for entire week
- clicking on an item should select it
- start w focus in first field
- entering any invalid number in break field wipes it out and its value is 0
- a total negative time makes the total go red to indicate an error
- valid times must be for in and out else no total is shown for that row (and its value is 0)
- fields 1 and 2 are interpreted as times and field 3 as a duration
- should understand time formats: 9, 9p, 9pm, 9:15, 9:15pm, 9:15p
- out time less than in time should result in error; highlighting in red
- if out is less than in, infer PM unless merdiem was explicitly stated
- replace the time with the normalized time so there is no confusion on what was selected
- limit the precision on any number to 2 decimal places
- BDD spec tests with Jasmine
- should return undefined for junk not 12am
- When visiting the page, should be able to see directions: …
- When visiting the page, should be one row displayed at first
- After filling out the last valid row, another is added
- Should be able to click a button to clear to start over (reload?)
- Deploy to host environment (Heroku)

Contact
-------
Post bugs and issues on [github].  Send other comments to John Lehmann:
first last at geemail dotcom or [@jplehmann]

[@jplehmann]: www.twitter.com/jplehmann
[github]: https://github.com/jplehmann/coursera/issues
[JQuery]: http://jquery.com/
[Moment]: http://momentjs.com/
[Bootstrap]: http://twitter.github.com/bootstrap/
[Jasmine]: http://pivotal.github.com/jasmine/
[Cucumber]: http://cukes.info/
[Knockout]: http://knockoutjs.com/
[Mustache]: https://github.com/janl/mustache.js/
[LESS]: http://lesscss.org/
[Heroku]: http://www.heroku.com/
[Rack]: https://devcenter.heroku.com/articles/static-sites-ruby
