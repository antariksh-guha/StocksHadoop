# StocksHadoop

### MapReduce Job To Compute Max Close Price By Stock Symbol ###

HDFS Input Location:
/user/hirw/input/stocks
HDFS Output Location (relative to user):
output/mapreduce/stocks

Delete Output Directory:
hadoop fs -rm -r output/mapreduce/stocks

Submit Job:
hadoop jar /hirw-starterkit/mapreduce/stocks/MaxClosePrice-1.0.jar com.hirw.maxcloseprice.MaxClosePrice /user/hirw/input/stocks output/mapreduce/stocks

View Result:
hadoop fs -cat output/mapreduce/stocks/part-r-00000