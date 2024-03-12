The "citibike_etl" file contains a code block that uses a for loop function to go through a series of sequentially numbered folders, pull their csv files, and merge them into a master dataframe. It's a handy tool when zip file downloads will break up time-sequential data across multiple folders.
Folders must be organized in numeric and/or calendar order for the function to work. 
Note: the numbering system for these folders started with "1", "2", etc. If the numbering system starts with "01", "02", etc. then a zero padding function must be added. 
The code uses concat instead of the append function because the latter kept causing a a weird TypeError claiming that the dataframe has no append function. 
