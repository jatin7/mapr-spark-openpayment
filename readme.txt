
Copy the data file from the project data folder to MapR Node in directory /user/user01/data/uber.csv

This example runs on MapR 5.2.1 with Spark 2.1  

You can run these examples in the spark shell by copy pasting  the code from the scala file in the spark shell after launching:
 
$spark-shell --master local[2]


Or you can run the applications with these steps:

Step 1: First compile the project: Select project  -> Run As -> Maven Install

Step 2: Copy the jar and data to the MapR Node  

To run the  standalone :

spark-submit --class payment.ETLPayment --master local[2] mapr-spark-payment-1.0.jar /user/user01/data/payments.csv

See the MapR-DB shell doc here https://maprdocs.mapr.com/home/ReferenceGuide/mapr_dbshell.html

You can run the notebooks by importing the json file into Zeppelin.

You can view the Zeppelin notebook with the viewer here 

https://www.zepl.com/viewer/github/caroljmcdonald/mapr-spark-openpayment/blob/master/notebooks/MapRSparkPayment.json

