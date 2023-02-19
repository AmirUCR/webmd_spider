# WebMD Spider

In this project, I use Python's Scrapy library to crawl https://www.webmd.com/drugs/2/index and extract the name and usage of all the drugs present. The code is ran using a Jupyter notebook or Google Colab or any other similar notebook interpreter. We export our crawled findings to a .csv file. The data acquired here may be used to cross-reference other medical datasets such as those from the CDC to perform EDA or other investigations on drug data.

I manually extracted each relevant XPath on WebMD's drug pages using Chrome DevTools (inspect element) to make the retrieval process more precise. Some pages on WebMD are different that others. For example, this page https://www.webmd.com/drugs/2/drug-63164/adderall-xr-oral/details is different from https://www.webmd.com/drugs/2/drug-7277/percocet-oral/details which means they are constructed using different HTML elements and thus require a custom XPath extraction. 

The spider extracts the following data from each drug page:

* Drug Name
* Usage
* Condition
* How to Use
* Generic Name
* Brand Name

Here's a snapshot of what the output .csv file looks like:

![Snapshot](https://github.com/AmirUCR/webmd_spider/blob/main/images/snapshot.png)

# Tools
* Python 3
* Scrapy https://scrapy.org/ and https://anaconda.org/conda-forge/scrapy
