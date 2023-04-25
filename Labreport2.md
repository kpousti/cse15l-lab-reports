Part 1: String Server

In this code segment, I have added an ArrayList to store the words in the query. This approach is more flexible as there is no predefined length for the words in the query, making it easier to handle.

When accessing the server without any queries given, the website displays as follows:

When accessing the server without any queries given, the website displays as follows:

With two queries, the website shows the results for both:


The main method being used here is the one shown above. Thanks to the if statements, it can easily respond to the requests sent to the server.

The URL of the server is the primary argument used within this method. This is because most of the requests made to the server are based on the URL link and changing it. The URL determines the use of the ArrayList and returns the statement.

It's worth noting that the ArrayList is the only relevant field in this class that affects the majority of the server. The ArrayList is updated with every query, which in turn updates the website to display all the string elements contained in the ArrayList.
