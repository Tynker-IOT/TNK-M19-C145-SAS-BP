Display the Data in a Table
======================
In this activity, you will combine the data from all the topics and display them on the table.


<img src= "https://s3.amazonaws.com/media-p.slid.es/uploads/1525749/images/11160110/Screenshot_2024-02-29_183824.png" width = "100%" height = "50%">


Follow the given steps to complete this activity.


1. Combine the data from the topics by using a join widget from the sequence section.


<img src= "https://s3.amazonaws.com/media-p.slid.es/uploads/1525749/images/11158065/SA2_join_widget.gif" width = "50%" height = "50%">


2. Convert the data from the join to an array by connecting a function widget to the join.


<img src= "https://s3.amazonaws.com/media-p.slid.es/uploads/1525749/images/11158426/pasted-from-clipboard.png" width = "50%" height = "50%">


* Convert the payload Object to an array.


~~~cpp
    msg.payload = [msg.payload]
    return msg;
~~~


3. Install the node-red-ui-table to the pallete.


<img src= "https://s3.amazonaws.com/media-p.slid.es/uploads/1525749/images/11158083/install_table_pallet.gif" width = "50%" height = "50%">


* Add the table widget from the dashboard section and connect it to the function AddToArray.


<img src= "https://s3.amazonaws.com/media-p.slid.es/uploads/1525749/images/11158438/pasted-from-clipboard.png" width = "50%" height = "50%">


4. Create a group named Data Table and add the table to the group.


* Set the width of the group to `20`.


<img src= "https://s3.amazonaws.com/media-p.slid.es/uploads/1525749/images/11158519/SA2_table_group.gif" width = "50%" height = "50%">


* Add a column for timestamps and columns for each MQTT topic. Set the size of the table to `20X6`.


<img src= "https://s3.amazonaws.com/media-p.slid.es/uploads/1525749/images/11158525/SA2_Add_Columns.gif" width = "50%" height = "50%">




* Save and run the code to check the output.
