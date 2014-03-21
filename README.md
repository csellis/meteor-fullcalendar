###FullCalendar jQuery Plugin - Meteor Smart Package

This is a the [fullcalendar jquery plugin](http://arshaw.com/fullcalendar/) as a meteor smart package.

###How to use?

1. Install [meteorite](https://github.com/oortcloud/meteorite)
2. `mrt add fullcalendar`

Check out the [fullcalendar api](http://arshaw.com/fullcalendar/docs/) for more details.

###To render in a template

1. Insert in resource_page.html:
```
<div id="calendar"></div>
```
2. Insert in resource_page.js:
```
Template.resourcePage.rendered = function () {
	$('#calendar').fullCalendar({
		header: {
			left: 'prev,next today',
			center: 'title',
			right: 'month,basicWeek,basicDay'
		},
    weekends: true, // will hide Saturdays and Sundays
    editable: true
});
}
```
    
