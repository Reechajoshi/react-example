# Details about the project

This app contains one component 
- SearchData - which calls a utils function `fetchSearchResultsFromAPI` which is dedicated to make a call to any given API
- This application is calling a public api provided by `Sanity.io` which returns cat breeds

# Running the applcation
- You can simply run the application using `npm start` command

# Goal
- The main goal of this pair programming session was to determine as many bugs as we can and fix them

# Bugs identified
The major bug identified was:
- On refreshing the page, the search term was not cleared. 
- To recreate this, simply type some search term `ab` and then refresh the page, it will still show results from `ab` however the textbox will be empty
- To make the search more real time, we need to replace useEffect with useRef