# To prepare data for Tempr:
- two files need to be created
- see code/processing/_PHET_a2_low_log.txt for an example
- all users for one group will be in one file
- the first line of a user file should be ========================================
- each proceeding line is one user action, in order
- NOTE: These lines will eventually be the id of an html element, and therefore may not contain illegal characters. "ID and NAME tokens must begin with a letter ([A-Za-z]) and may be followed by any number of letters, digits ([0-9]), hyphens ("-"), underscores ("_"), colons (":"), and periods (".")."


# To use Tempr:
- create two files as specified above, one for each group of users
- edit the "USER ENTERED SPECIFICATIONS" section of code/processing/parse_get_temporal_freq.py
- you will need to specify the name of each of the two files above, a name for the data, and a two letter abbreviation for each group
- within the code/processing directory, run parse_get_temporal_freq.py with python 2. This could take a few minutes depending on the size of the log files, but you can observe the progress in the json_files subdirectory. ALL_ACTIONS_x.json files need to be created for x in 1-20.
- open index.html in firefox


Video for an older version of the project can be found at: https://www.youtube.com/watch?v=kkeWC6rLBe4
