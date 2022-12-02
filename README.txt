Student Names - Student Numbers:
-----------------------------------------
REDACTED
_________________________________________

Instructions for use of Program:
-----------------------------------------
Launch Jupyter notebook and locate the file "IR_Search_Engine_CH_PK.ipynb", it will be in the same directory 
as this readme

Once the file is open click the 2 arrows to the right of the run command to reset the kernel and run the whole program
(Alternatively run each cell one at a time)

The first cell will import and download the necessary libraries, if these already exist it will skip them.

A majority of the cells contain functions required for the program to run. You can ignore these for now.
(but make sure you run each of them if you're running each cell individually!)

Scroll down until you see the header "Main Program - Run in order"
Run the cells below these in order, following prompts along the way. 

You will need to point the program to the directory where the html files are contained

The directory can be typed either as:
/this/is/the/directory/currentDirectory/marvelWiki 
or 
marvelWiki if the folder is contained within the current directory

if you simply hate having to input it in a text box you can give it as an argument to the build function
e.g build("marvelWiki")

This will build the index, and it will save 3 JSON files to your current directory. These include:
vocab.json
postings.json
docids.json

Once that cell has finished running, you can run the cell below it. This is the main search engine
where you will type your queries.

If you'd prefer to have your queries returned as a List, type forceList and press enter. Then type your query.
If not, simply type in your query and press enter. It should be displayed line by line below.
Once you're finished you can type quit and it will stop running that cell.

-------------(IMPORTANT NOTE)------------
Due to the way IPython works, occasionally the query box will disappear, in which case you must press the STOP 
button at the top of the screen and then press the PLAY button on the cell to run the query box again
-----------------------------------------

Below these cells are some test cells, these ensure that everything is working nicely.

If you run the test_iteration_counter cell it will run through the query "ironman" 5000 times and give you
the average time it takes to run that query that many times. Its useful for checking efficiency.
(you can change the input by changing "ironman" to anything of your choice)

Below this is a function tester.
**READ THE WARNING AND SAVE THE THREE JSON FILES ELSEWHERE BEFORE TRYING TO RUN IT**
It will go through every function and return either True or False depending
on whether the function worked as intended or not.

To get this cell to run you must type y in the text field it prompts you with. This is to stop you from accidentally
overwriting the three JSON files created earlier. However it does not alter the main functionality of the program,
and the main() cell should still be able to run after the fact.

-----------------------------------------