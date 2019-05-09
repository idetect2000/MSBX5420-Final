# MSBX5420-Final

The goal of this project is to create a recommendation system for online purchases. This was achieved by collecting over 40,000 invoice records between 2010 - 2012. These invoices gave insigt into what items are frequently puchased together. Using this information in conjunction with Elastic Search's built in aggregations we were able to come up with an efficent and effective reccomendation system.

It is not enough to just suggest items that were puchased together with some frequency. For instance, if people frequently purchased The Office DVD box set and water together, we can logically see that there is no corralation between the two. Water is just something that is needed. Wich is seperate from the want to watch The Office". This was accounted for through the use of "highly correlated words" and "significant terms" which weed out the items that were purchased together but are not correlated. 

The input for the recomendation system is a single stock code, if you purchase stock code 22295, the recomendation system will return for you the stock codes of items that are frequently purchased with stock code 22295.

