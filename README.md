# BellyButton

## Backgroun
Roza has a partially completed dashboard that she needs to finish. She has a completed panel for demographic information and now needs to visualize the bacterial data for each volunteer. Specifically, her volunteers should be able to identify the top 10 bacterial species in their belly buttons. That way, if Improbable Beef identifies a species as a candidate to manufacture synthetic beef, Roza's volunteers will be able to identify whether that species is found in their navel.

## To Run The HTML Correctly
In he directory where samples.json and index.html. Open the command line (Terminal or Git Bash) and type the following:

  python -m http.server
  
You should see the following message in the command line:

  Serving HTTP on 0.0.0.0 port 8000 (http://0.0.0.0:8000/) ...
  127.0.0.1 - - [30/Oct/2019 13:23:53] "GET / HTTP/1.1" 304 -
  
Navigate to the given port number in your browser: localhost:8000 .

## Web Page dashboard look like
![screenshot](https://github.com/hayden0098/BellyButton/blob/main/images/screenshot.jpg)

* Dropdown menu on the left is for selecting the Test Subject ID number.
* Bar Chart display the top 10 bacterial species (OTUs) when an individual's ID is selcted. X-axis = ID, Y-axis = sample values
* Bubble Chart display the following when individual's ID is selcted:
  1. The otu_ids as the x-axis values.
  2. The sample_values as the y-axis values.
  3. The sample_values as the marker size.
  4. The otu_ids as the marker colors.
  5. The otu_labels as the hover-text values.
* Gauge Chart displays the weekly washing frequency's value, 0-19 on the progress bar
