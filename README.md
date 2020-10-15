# Define
A dictionary lookup and appending script in python3

## Installation
You may already have python installed on your machine! However:
python3 installation instruction can be found [here](https://wiki.python.org/moin/BeginnersGuide/Download)

## Clone
Clone the repository using git:
`git clone https://github.com/wiregolem/define.git`
or with Github CLI:
`gh repo clone wiregolem/define`

## Usage
`python3 define [args]`
where args represents n number of words to be looked up in the dictionary file

## Expected behavior 
1. The script will loop over each argument, checking for it's definition in the supplied dictionary file
2. With every iteration, if a word is found, the word and it's definition will be output to console
3. This loop ends when the dictionary file does not contain a the specified word, instead:
   - The word will be displayed to console
   - followed by the prompt "Word not defined, please enter definition or press return to skip"
     - If return is pressed without character or string input the script terminates
   - the script will redisplay the word being defined along with the user supplied definition and the prompt:
     - "Are you sure? case sensitive"
     - "S submit, R retry, D discard"
       - `S` appends the key value pair, it's word and definition, to the dictionary file exiting with the successful message "Entry submitted"
       - `R` reprompts for the definition, as done invalid input
       - `D` discards the user supplied definition, making no changes to the file, and terminates the script


