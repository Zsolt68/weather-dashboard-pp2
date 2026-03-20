# Weather-Dashboard - Testing

-----

## Contents

* [Introduction](#introduction)
* [Automated Validation](#automated-checks-and-validation)
    * [W3C Validator](#w3c-validator)
    * [Lighthouse](#lighthouse)
    * [JSHint](#jshint)
* [Manual Testing](#manual-testing)
    * [Full Testing](#full-testing)
* [Bugs](#bugs)
    * [Solved Bugs](#solved-bugs)
    * [Known Bugs](#known-bugs)

-----

## Introduction

Here, I developed a testing plan to make sure that the weather-dashboard or website was functioning as intended. 

I ran my code through all validation and accessibility checkers noted below and have included screenshots of the results in this document. I also manually checked every feature of the site to ensure that it was working as intended and have included the results of this testing in this document.

-----

## Automated Checks and Validation

This automated testing section contains all testing that has been run through a program to produce validation and performance insights.

### W3C Validator

[W3C](https://validator.w3.org/#validate_by_input) was used to validate the HTML and CSS for the site via direct text input. Result: Document checking completed. No errors or warnings to show.

### Jigsaw Validator
[Jigsaw](https://jigsaw.w3.org/css-validator/validator$link)  was used to validate the CSS for the site via direct text input. Result: Congratulations! No Error Found.

### Lighthouse

The Lighthouse tool within the Chrome Developer Tools has been used to test performance, best practices, accessibility, and SEO. Desktop and mobile tests have been run for each page.

| | Performance | Accessibility | Best Practice | SEO |
| :---: | :---: | :---: | :---: | :---: |
| Desktop | 100 | 99 | 100 | 89 |
| Mobile | 100 | 99 | 100 | 89 |

### JSHint

[JSHint](https://jshint.com/) was used to test the JavaScript file in this project.

The JavaScript file tested with JSHint returned no errors.

### Testing Table


Feature	Expected Result	Test Performed	Result	Pass/Fail
Search bar	User enters city, weather loads	Typed “Dublin”	Weather displayed	✔️ Pass
Invalid city	Error message shown	Typed “asdfgh”	Error displayed: City not found, Try again.	✔️ Pass
Recent searches	Buttons appear and work	Clicked for 8 saved city	Weather loads	✔️ Pass
5‑day forecast	Shows 5 cards	Searched multiple cities	All cards visible	✔️ Pass
Responsiveness	Layout adjusts	Tested on mobile/tablet	Works correctly	✔️ Pass
API connection	Data loads	Checked network calls	Successful	✔️ Pass


### Testing User Goals

> * Search for a city and display the city's name and current temperature.

The weather dashboard is designed to be a simple way to search for a city name, then to display the city's temperature and 5-day weather forecast.

> * Be able to collect multiple/8 cities' searches and display them on the weather dashboard.

### Testing Summary

Functional Testing
Search functionality

API response validation

DOM updates

Error handling

Recent search behaviour

✔️ Responsiveness Testing
Mobile

Tablet

Desktop

✔️ Browser Compatibility
Chrome

Firefox

Edge

Safari

✔️ Validator Testing
W3C HTML

W3C CSS

JSHint


### Full Testing

Full testing was performed on the following devices:

* Laptop
  * HP Pavilion - 15

* Mobile
  * Samsung Galaxy S25+
 
 Desktop device tested the site using the following browsers:
 
 * Google Chrome
 * Mozilla Firefox
 * Opera
 * Microsoft Edge


   ## Bugs

### Solved Bugs

| # | Bug | Description | Fix implemented | Fixed? |
| --- | --- | --- | --- | --- |
| 1 | Layout breaking on mobile | Cards overflowed screen | Added responsive CSS | __Yes__ |
| 2 |  Dublin's temperature is wrong | The app does not dislays the right temperature for Dublin, Ireland | I cannot fix this because it is the wrong data from the OpenWeather API> ineed to change the API for this project to rectify the issue | __No__ |


### Known Bugs

The Weather Dashboard does not display the right temperature for Dublin because the OpenWeather API does not render the weather details correctly for it. It is not a bug in my coding.

<sup><sub>[*Back to top*](#contents)</sup></sub>

-----
