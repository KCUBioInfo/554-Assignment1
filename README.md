#BIOS 554- Assignment 1


For this assignment, you will be programming in the Bash scripting language and using Unix terminal commands. If you use Mac OS or Linux on your computer, you can access the terminal directly. Otherwise, create an account on pythonanywhere.com and open a BASH terminal, load a linux operating system image on Docker (e.g. Ubuntu), or install the Bash terminal for Windows on your computer. You should submit the .sh files generated as part of this assignment using Github. You should also submit a .csv file that you used to test problem 5 (i.e. make up a data file) and all of the .json files generated as part of problem 6. The Github repository for this assignment is here:
1)	Write a Bash program that prints “Hello World” to the terminal when it is run.
2)	Write a Bash program that prints out all of the files in a directory with a given file extension. This extension will be provided as an argument from terminal when the script is called.
3)	Write a Bash program that prints out the contents of a text file to terminal. The name and path of the text file will be provided as an argument from terminal when the script is called.
4)	Write a Bash program that prints out all of the words in a text file that begin with a vowel – one per line. The name and path of the text file will be provided as an argument from terminal when the script is called.
5)	Write a Bash program that reads a csv of research participant data (ID, Age, Sex, and various measurements). The first row of this csv will contain the labels ID, Age, Sex, and the names of each measurement. From this csv, create a folder for each participant ID. Within this folder, create a file whose name follows the format “ID-MeasurementName.txt” for each of the measurements in the csv. This file should contain the appropriate value for that participant from the csv. The name and path to the csv input file will be provided as the first argument in terminal when the script is called, the output path where the folders should be created will be the second argument. Note that you may need to delete files in between tests. Example Input:

```
ID,Age,Sex,Measurement1,Measurement2, …, MeasurementN
ABCDEFG,32,M,73,42,…,105
1234567,100,N,100,101,…,3
89101112,5,F,12, 14,…,18
HIJKLMNO,17,M,1,3,…,13
```

6)	Write a Bash program that reads through the file structure created in problem 5. This script should generate a valid JSON file (ID#.json) for each participant based on the directory structure and file contents. For example:

```
{
	“ID”: “ABCDEFG”,
	“AGE”:”32”,
	“SEX”:”M”,
	“Measurement1”:”73”,
	“Measurement2”:”42”,
	…
	“MeasurementN”:”105”
}
```

