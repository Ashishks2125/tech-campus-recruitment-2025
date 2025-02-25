Steps to Solve the Problem
1. Read the ZIP File
Use the zipfile module to open and read the contents of the ZIP archive.
Identify the .log files within the archive.
2. Perform a Binary Search
Since the log file is large, we avoid scanning it linearly and instead perform a binary search based on timestamps.
The idea is to seek through the file and narrow down to the first occurrence of target_date.
3. Extract and Write the Logs
Once the first occurrence of target_date is found, extract the logs until we reach the next date.
Write the extracted logs to a new file.
