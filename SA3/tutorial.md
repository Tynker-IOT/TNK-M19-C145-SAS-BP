Display Past Data in the Table
======================
In this activity, you will display the historic data in the table.


<img src= "https://s3.amazonaws.com/media-p.slid.es/uploads/1525749/images/11157361/SA3.gif" width = "100%" height = "50%">


Follow the given steps to complete this activity.


1. Retrieve the recent data by accessing the data from the flow.
* Double click on the AddToArray function, replace the program with the below program.
   ~~~js
    var tableData = flow.get("savedData") || []
   ~~~


2. Include timestamp to recent data by getting the date and converting to human-readable format.


   ~~~js
    msg.payload["timeStamp"] = new Date().toLocaleString()
   ~~~


3. Place the recent data at the top of the table by shifting the data to the top.
   ~~~js
    tableData.unshift( msg.payload)
   ~~~


4. Place the recent data at the top of the table by shifting the data to the top.
   ~~~js
    msg.payload = tableData
    flow.set("savedData", tableData)
    return msg;
   ~~~


* Save and run the code to check the output.
Display Past Data in the Table
======================
In this activity, you will display the historic data in the table.


<img src= "https://s3.amazonaws.com/media-p.slid.es/uploads/1525749/images/11157361/SA3.gif" width = "100%" height = "50%">


Follow the given steps to complete this activity.


1. Retrieve the recent data by accessing the data from the flow.
* Double click on the AddToArray function, replace the program with the below program.
   ~~~js
    var tableData = flow.get("savedData") || []
   ~~~


2. Include timestamp to recent data by getting the date and converting to human-readable format.


   ~~~js
    msg.payload["timeStamp"] = new Date().toLocaleString()
   ~~~


3. Place the recent data at the top of the table by shifting the data to the top.
   ~~~js
    tableData.unshift( msg.payload)
   ~~~


4. Place the recent data at the top of the table by shifting the data to the top.
   ~~~js
    msg.payload = tableData
    flow.set("savedData", tableData)
    return msg;
   ~~~


* Save and run the code to check the output.
