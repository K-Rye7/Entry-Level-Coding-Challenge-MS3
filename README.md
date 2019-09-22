# Entry-Level-Coding-Challenge-MS3
Coding test given by MS3 

Summary:
	The purpose of this repo is to read CSV files, parse through the lines (checking for inconsistencies or blank spaces within the CSV while adding those lines
	to a bad CSV file), and insert the "good" lines (or records) into a SQLite database. The application creates the SQLite database and table that it adds to.
	This is all part of a coding challenge given by Mountain State Software Solutions. 

Steps to get this running
	1) Download all the files needed within the repo
	2) Make sure you have the CSVReader.jar and the library folder 
	3) Open command prompt
	4) Change directories to wherever you downloaded the files with CSVReader/dist at the end
	5) Execute the application

Overview:
	My initial approach to this project was to get the CSV reader functioning first. I wanted to be able to know for sure how to go through the CSV and take data from it. 
	I got that part working and proceeded to find a way to weed out the bad entries while adding them to their own separate .csv file. It is very apparent that I got a lot
	of my code from various different places through google searches of the problems. Databases are not my strong suit, so I did that part last. Assuming that the database
	I was supposed to be accessing was one I needed to create myself I got to work on that next. I was able to successfully? create the database through what I assume are 
	conventional methods with SQLite. I then created another class to make the table I needed within the database so I would have something to add all my CSV data to. 
	The last part I worked on was taking the data from the CSV and putting it into the SQLite database. Initially I wanted to just create another "good" .csv file and 
	just put all of that data in, but I realized that would be wildly inefficient so I decided to try to input the csv data into the database within the CSVReader class 
	that already parses through the CSV for me. I had trouble getting it to work, but I think It should at least compile. I didn't know what the data was for, or what the
	titles of the columns were supposed to be in the CSV since all I was given were letters for that. That is why every entry in the database is a string. I didn't want
	to make assumptions on what the theoretical client wanted the data to be or do since I didn't have the information for that, so I left everything as a string. After
	doing that it was easy to fit it into the existing code that I had before. I only had to make a nested try to make it work. 
	
	Given more time to reacclimate  myself with Java, and to learn SQLite more, I would probably have started with getting the database stuff working first, then moving on to 
	the csv implementation into the database 

That should conclude everything within the challenge. I would like to thank whoever is reading this for taking the time to look at everything in here. 
	