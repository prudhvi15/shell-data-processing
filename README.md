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
1. ```tr ' ' '\12' < data.txt | sort | uniq -c``` is used to pipe the sorted output to uniq -c to count.
1. ```tr ' ' '\12' < data.txt | sort | uniq -c | sort -nr``` is used to pipe the reduced output that is after getting unique words to sort with -nr flag.
1. ```tr ' ' '\12' < data.txt | sort | uniq -c | sort -nr > result.txt``` is used to redirect the output to result.txt file.
1. Up arrow in bash shell is used to get previous commands we used.

#### Important bash commands
1. To redirect all the contents of our directory ```ls > filename.txt``` command is used(file name is of our choice).
1. we can use two arrows(>>) to append instead of overwriting.
1. ```ls``` command is used to list all the contents of the default directory.
1. we can use cat command to diplay the contents of the file.
Example: ```cat temp.txt```
