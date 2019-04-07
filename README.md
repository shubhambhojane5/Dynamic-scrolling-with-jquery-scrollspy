# Dynamic-scrolling-with-jquery-scrollspy

## Features

1. Overview
1. Setup
2. Links
3. Probelm defination and code sample
4. References

###### Overview

Dynamic scrolling with jquery scrollspy allow developer to load full data at once without any challenges. Jquery scrollspy detects viewport so that we can add dynamic HTML without any performances issue. It also allow to do custom changes in scrollspy events.

###### Setup

Inclue jquery and jquery scrollspy in project. Scrollspy provide viewport on window by default but we can modify it.

###### Links

[https://plugins.jquery.com/scrollSpy/]

###### Probelm defination and code sample

We have more than 500+ row with 20+ columns and every column have custom html control(input, datepicker etc) and every controls are editable. If we try to load all this row at once, will face performance issues while scrolling and editing. So in that case jquery scrollspy will come in role to help to load all data at once without any performance issue. Just load blank table with row id's, Scrollspy detects the viewport and allow developer to add dynamic HTML on runtime using predefined method like scrollspy:enter and also remove the HTML which are not present in viewport using scrollspy:exit.

- First we have change the default behaviour of scrollspy viewport to table viewport.
- $('#table_id tr').on('scrollSpy:enter', function () {
// To DO
// This method remove the row of table which are not present in table viewport.
});
- $('#table_id tr').on('scrollSpy:exit', function () {
// To DO
// This method add the row of table which are present in table viewport.
});
- $('#table_id tr').scrollSpy();

###### References

* https://plugins.jquery.com/scrollSpy/

