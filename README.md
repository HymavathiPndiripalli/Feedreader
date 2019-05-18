# Feedreader Testing

## how to clone the Project

-   Clone the repository which is provided by the Udacity <https://github.com/udacity/frontend-nanodegree-feedreader.git>

## Structure of the Project

the following files are extracted:
            1\. css/icomoon.css
            2\. css/normalize.css
            3\. css/style.css
            4\. fonts
            5\. jasmine/spec/feedreader.js
            6\. js/app.js
            7\. index.html
            8\. README.md

## How to run the application

-   open index.html file in your favourite browser

## What I have done in this Project

-   `suite` -A test suite begins with a call to the global Jasmine function describe with two parameters: a string and a function. The string is a name or title for a spec suite - usually what is being tested. The function is a block of code that implements the suite.

-   `spec` - Specs are defined by calling the global Jasmine function it, which, like describe takes a string and a function.

-   Inside the feedreader.js file I have implemented the following statements:
    -   `RSS Feeds` suite code have already provided
        -   'are defined' spec code is provided to check that allFeeds variable is defined or not
        -   I have created 'get all urls here' spec to ensures that each feed in allFeeds object has a URL defined and that the URL is not empty
        -   I have created 'get all names here' spec to ensures that each feed in allFeeds object has a name defined and that the name is not empty
    -   I have created `The menu` suite
        -   I have created 'hidden or showing' spec to ensures the menu element is hidden by default.
        -   I have created 'visibility of icon' spec that ensures the menu changes visibility when the menu icon is clicked. This test have two expectations:     
            -   the menu display when clicked
            -   it hide when clicked again
    -   I have created `Initial Entries` suite
        -   I have created 'work of loadfeed' spec that ensures when the loadFeed function is called and completes its work, there is at least a single .entry element within the .feed container. Here loadFeed() is asynchronous so I used the Jasmine's beforeEach and asynchronous done() function
    -   I have created `New Feed Selection` suite
        -   I have created 'loading new feed' spec that ensures when a new feed is loaded by the loadFeed function that the content actually changes

## Conclusion

-   I have learned how to use jasmine to pass test cases based on requirement of an application
-   I have learned event handling and DOM manipulation
-   I have improved my testing and analyzing skills
