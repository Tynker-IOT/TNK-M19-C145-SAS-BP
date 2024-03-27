Fix the Bug
======================
In this activity, you will debug the code to display multiple records in the table.


<img src= "https://s3.amazonaws.com/media-p.slid.es/uploads/1525749/images/11199573/pasted-from-clipboard.png" width = "100%" height = "50%">


Follow the given steps to complete this activity.


1. Fix the bug by editing the code in the `AddToArray` function.
~~~js
    var tableData = flow.get("savedData") || []


    msg.payload["timeStamp"] = new Date().toLocaleString()


    tableData.unshift( msg.payload)


    msg.payload = tableData


    flow.set("savedData", tableData)


    return msg;
~~~


* Save and run the code to check the output.
