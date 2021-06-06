# Crawler
A Web crawler designed to download .xml files from the urls it visits. Python and it's libraries are used.
Jupyter notebook has been used.

## URL Frontier 
1) Takes in seed urls and implements front queue and back queues. 
2) Each thread will access the link from back queue.
3) A priority queue is maintained which stores the time when the backqueue can be accessed by a thread.
4) To maintain politeness each thread waits 15 seconds before sending another request.

## Filter Urls
1) It checks if the link is valid.
2) Converts relative link to absolute link.
3) If Robot file contains * then can fetch the file.
4) Removes duplicate urls.
5) Download .xml of html pages in current directory.

## Run Crawler
1) Creates Threads and intializes limit documents.
2) Implements the process_data function that each thread executes
3) Saves the mapping of url to filename as "urlTodocid.txt".

## Running Code
![CodeImage](https://github.com/froheel/Crawler/blob/main/RunningCode.PNG)
