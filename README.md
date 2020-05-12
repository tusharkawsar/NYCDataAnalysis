# NYCDataAnalysis

NBviewer Link: https://nbviewer.jupyter.org/gist/tusharkawsar/6ebafcbf4a02ed84019192df3326104c

In this assignment, we explore the datasets of established businesses and their applications for a licence in NYC. The data sets are well known and we will need to join them together on a logical primary key. However, they are not clen and there are a lot of missing values as well as misplace/wrong attributes.

Therefore, I have decided to make use of another dataset to make our lives easier. This third dataset contains zip codes against borough names in NYC. Therefore, this dataset can help in the first two tasks.

Source: https://www.kaggle.com/kimjinyoung/nyc-borough-zip

For Task 1, we use the License Application (df\_application) dataset as well as the new zip code (df\_zip) dataset. We simply go through df\_application and collect the business application turnaround time for each of the boroughs. We then find the borough which takes the longest to accept applications.

For Task 2, we make use of the program in Task 1 and directly dive into the associated borough. This time, we find out turnaround time for different business categories and find the maximum amongst them.

For Task 3, we do a similar procedure. We make use of a custom function to find out application and renewal denial rates in all five boroughs.

For Taks 4, we need the status attribute from Legally Operating Business (df\_business) dataset. We join the provided datasets together to find which garage/parking related business are going to be expired (application-wise) in 2020. We also see when their last application-related activity was. In the end, we write this information in a CSV file.

I used a Jupyter Notebook to write my codes and functions. I used pandas dataframe to contain the huge data sets since pandas is known for efficiently handling large data. 


