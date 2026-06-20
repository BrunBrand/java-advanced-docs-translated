# Find the Median in 500 Million Numbers

Finding the median of a massive dataset can be done with a **value range** approach. If numbers are integers with a known range, perform a counting sort: count how many numbers are less than each value until you reach the median position【386122166985391†L41-L66】. Another method is **quick select** with external storage or sampling.
