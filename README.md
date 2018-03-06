# Remote-Code-Publisher-OOD(Object Oriented Design):

### Purpose:

A Code Repository is a Program responsible for managing source code resources, e.g., files and documents. A fully developed Repository supports file persistance, managment of versions, and the acquisition and publication of source and document files. A Remote Repository adds the capability to access the Repository's functionality over a communication channel, e.g., interprocess communication, inter-network communication, and communication across the internet.

In this project I have developed a Remote Code Repository, local Client, and communication channel that supports client access to the Repository from any internet enabled processor.

The communication channel uses sockets and support an HTTP like message structure. The channel supports:

* HTTP style request/response transactions.

* One-way communication, allowing asynchronous messaging between any two endpoints that are capable of listening for connection requests and connecting to a remote listener.

* Transmission of byte streams that are set up with one or more negotiation messages followed by transmission of a stream of bytes of specified stream size.

The Remote Code Repository:

* Supports check-in, check-out, versioning, and browsing.

* Transfer source code text files to and from a local Client.

* Support defining dependency relationships between code packages saved in specific repository folders, based on the functionality you provided.

* Supports storing package metadata in the NoSql database.

Clients of the Remote Code Repository provide a Graphical User Interface (GUI) with means to:

* Upload one or more source code text files to the Remote Repository, specifying one or more categories with which those files are associated.

* Display package categories, based on metadata stored in the NoSql database.

* Display collections of filenames based on queries defining categories, filenames, dependencies, and versions.

* Display all of the files in any category that have no parents.


### How to operate the GUI
#### File List Screen:

* SELECT DIRECTORY: Opens a folder on browser click and select the files, they wwill be seen on the list box.

* SHOW SELECTED ITEMS: This just shows the selected files on the list box

* SEND FILES: Sends only the selected files to the server(You have to select)
FOLDER: "../SERVER-RCVD-FILES/(Whatever category)

* ComboBox: Select Category to send the filess to, default (Received Files 1)

* DOWNLOAD: Download .html files to the client Side.
FOLDER: "../CLIENT/(Whatever Category)

NOTE: You can see the file you send to the server on the send message screen.

Thank you.
