# webcrawler_colly

## Assignment for webcrawling:
This assignment using Colly to extract paragraph text from webpage and write extracted data into JSON line file.

## Output:
The output are text content collected from provided URL. Along with text content, the output file also print "url", "title", "text"(which is the main content).

## Issue:
Several issues in this simple application. As colly runs concurrently, the var data may cause data discrepency.

## Performance:

Compare to Python crawler, the experiements run purely on terminal with "time python run-articles-spider.py" & "time go run main.go"


The outcome: 

Python run-articles-spider.py  5.53s user 1.79s system 31% cpu 23.178 total


go run main.go  1.01s user 0.97s system 65% cpu 3.009 total.


The problem of this experiment is that the go code extract only text content which is inaccurate measurement comparing to Python, but still shows a huge difference in use of two languages.
