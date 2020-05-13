# shell-data-processing
### The following are the commands used to retrieve and process the text data.
#### To retrieve text
1. URL I used is "https://en.wikipedia.org/wiki/Big_data"
1. Curl command used to return the page text: ```curl "https://en.wikipedia.org/wiki/Big_data"```
1. Curl command used to get data and output to a file: ```curl "https://en.wikipedia.org/wiki/Big_data" -O data.txt```

#### To process text data
1. Bash commands are used to process the text.
1. ```tr ' ' '\12' < data.txt``` is used to divide each line into individual words.
1. Pipe is defined as sending the results of one command as input to another command.
1. ```tr ' ' '\12' < data.txt | sort``` is used to sort the text.
1. ```tr ' ' '\12' < data.txt | sort | uniq -c``` is used to pipe the sorted output to uniq -c to count. "-c" flag is to check for sorted iput.
1. ```tr ' ' '\12' < data.txt | sort | uniq -c | sort -nr``` is used to pipe the reduced output that is after getting unique words to sort with -nr flag.
1. ```tr ' ' '\12' < data.txt | sort | uniq -c | sort -nr > result.txt``` is used to redirect the output to result.txt file.
1. Up arrow in bash shell is used to get previous commands we used.
1. ```sort --help``` displays mandatory arguments that are to be used while sorting with bash commands.
1. "-n" flag is used to sort the data by comparing with numerical value.
1. "-r" flag is used to reverse the results of comparisons.
1. Only one dash is used when it is a single letter flag.
1. Two dashes are used when it is a flag with more than one letter.

#### Important bash commands
1. To redirect all the contents of our directory ```ls > filename.txt``` command is used(file name is of our choice).
1. we can use two arrows(>>) to append instead of overwriting.
1. ```ls``` command is used to list all the contents of the default directory.
1. we can use cat command to diplay the contents of the file.
Example: ```cat temp.txt```
