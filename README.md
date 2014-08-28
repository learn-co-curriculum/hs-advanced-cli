NOT ALLOWED TO CD ANYWHERE 
ALL COMMANDS MUST BE WRITTEN IN A SHELL SCRIPT

# Advanced Command Line and Shell Scripting

You've just been hired by your local grocery store to stock all of the shelves with a delivery that has come in from the warehouse. Congratulations on your new job.

## Part 1: Write a shell script.

You've learned about the different commands in your terminal (ls, mv, rm, mkdir, touch, etc), but now we're going to learn how to string these commands together by using bash scripting. A bash script is essentially a file with a set of instructions inside of it that when called from the command line will run the commands in the order in which they are written in the file. For example, in your development directory create a file called `test_script.sh`. Open this file up in a text editor (such as Sublime). Add to the contents of the file:

```
ls;
mkdir this_is_a_directory_made_in_a_script;
mkdir another_directory
touch this_is_a_directory_made_in_a_script/first_file.txt;
touch this_is_a_directory_made_in_a_script/second_file.txt;
mv this_is_a_directory_made_in_a_script/second_file.txt another_directory

```

Save and close the file and then run it in your terminal by typing `sh test_script.sh`. This will run all the commands in this bash script and if you look at your files once this is done (using `ls`), you'll find the two directories with their corresponding files that were created by running the script. Cool, eh?

### Challenge 1:
Using the mini-lesson above, write a bash script that will put all of the files in the devlivery directory in their right locations. As part of the challenge:
-You cannot CD into any directories, you must stay in the root directory of the project.
-All commands should be written in a shell script called `stock_supermarket.sh`

## Part 2: Search for code inside files
