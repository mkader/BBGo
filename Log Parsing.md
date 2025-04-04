GREP - Searches any given input files, selecting lines that match one or more patterns.

CUT - cuts out selected portions of each line from each file and writes them to the standard output.

SED - reads the specified files, modifying the input as specified by a list of commands.

AWK - scans each input file for lines that match any of a set of patterns.

SORT - sorts text and binary files by lines.

UNIQ - reads the specified input file comparing adjacent lines and writes a copy of each unique input line to the output file.

These commands are often used in combination to quickly find useful information from the log files. For example, the below commands list the timestamps (column 2) when there is an exception happening for xxService.

grep “xxService” service.log | grep “Exception” | cut -d” “ -f 2

<img src="https://substack-post-media.s3.amazonaws.com/public/images/c28f0cbc-a40f-4bdb-88be-f2a0ab900bbc_1280x1683.jpeg">

