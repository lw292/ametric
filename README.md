# Author-Level Metrics

This script generates the following author-level metrics from reference data files in the BibTeX format:
* **_h_-Index**: A scholar with an *h*-Index of *h* has published at least *h* papers, each of which has been cited at least *h* times.
* **Normalized _h_-Index**: A scholar with a Normalized *h*-Index of *nh* has published at least *nh* papers since the first paper, each of which has been cited at least *nh* times.
* **_m_-Index**: A scholar's *m*-Index is calculated as the *h*-Index divided by the number of years since the first paper.
* **Normalized _m_-Index**: A scholar's Normalized *m*-Index is calculated as the Normalized *h*-Index divided by the number of years since the second paper.
* **Average Citation Count**: The average number of times a scholar's papers have been cited.
* **Normalized Average Citation Count**: The average number of times a scholar's papers, excluding the first paper, have been cited.
* **Date of Second Publication**: The year in which a scholar's second paper was published.

## Installation

Before you can run the script, you will need to install some dependencies.

First, make sure you have a Ruby environment. Start a terminal window and run:
```
	ruby -v
```

Second, make sure that the Ruby gem `bibtex-ruby` is installed:
```
  gem install bibtex-ruby
```

If you use the Ruby gem bundler utility, running this command will install `bibtex-ruby` automatically:
```
  bundle install
```

## Running the Script

Make sure that your ".bib" files are located in the "data" subdirectory, and then run:
```
  ruby ap.rb
```
That should output a ".csv" file in the "results" subdirectory.

## Cleaning the Data

This script has been tested to work with reference data from the Web of Science and Scopus. If you have data from both of these resources, you will need to remove possible duplicates in your data. We recommend using EndNote to deduplicate your reference data.

To re-export deduplicated data from EndNote, please use the included "BibTeX_Export_Impact" style.

More coming soon ...
