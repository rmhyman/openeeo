# openeeo
There has been a lot of talk about diversity in Silicon Valley.  Companies have started to release data about their demographic makeup, and have started to release their [EEO-1 reports](https://www.eeoc.gov/employers/eeo1survey/index.cfm) along with their own data analysis.
Both of these formats are not in a format for the public to perform their own data analysis since the EEO-1 reports are typically released as images or PDFs
And the data used for their findings are not made public.  Also the EEO-1 report link is sometimes a static link on the company's page where they can just update that link to the latest EEO report.
This repo is for placing EEO reports in a Analyzable format for Open Data Analysis and having the data for future reference.  

##Process
After accumulating the EEO reports that I was able to find(located [here](tech/originals)), they were not in a format that it is easy to parse.  To extract the text I used [OnlineOCR](http://www.onlineocr.net/) to extract the text.  There were a few (I encountered 3 so far) where the text did not extract well.  For those cases, I extract the numbers.  There are other tools that can be used to extract from PDFs and Images.  [Tessaract](https://github.com/tesseract-ocr) is another tool that I came across but have not used yet.  The [textract](https://pypi.python.org/pypi/textract) python module also can extract text.
The text format that I used can be found [here](tech/txt_files).  I formatted the data using the code found in the Ipython notebook.  This generates the csv files found [here](tech/csv).

##Purpose
I hope that this database will continue to grow with EEO-1 reports not just from the tech industry but all other industries as well.  I would love for others to contribute to this repo and expand it so that we have as much open data as possible.  I've also filed a request with [data.gov](https://www.data.gov/) so that they can provide a database such as this for public use.
