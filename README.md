<h1 id="eng" align="center">Firebase API Example</h1>

<br>

This project aims to develop an API that accesses the Firebase database using the Python Flask library. Firebase is a cloud-based database that allows users to store, synchronize, and share real-time data. The API provides users with the ability to add, view, and delete data.

<br>

## Features of the Project:

-   Ability to read data from the database
-   Ability to add data to the database in JSON format
-   Ability to view tables in the database
-   Ability to delete tables in the database

<br>

## Libraries Used in the Project:

-   ### [Firebase](https://pypi.org/project/firebase-admin/)

-   ### [Flask](https://pypi.org/project/Flask/)

<br>

## Project Setup

```shell
git clone REPO_URL
cd firebase-api
```

## Installation

After creating a project on Firebase, go to the **Project settings** tab, select Python from the service accounts, and click the **Generate new private key** button to download the API credentials. Rename the downloaded file to **key.json** and place it in the **firebase/api** folder.

<hr>

### Installing the required libraries and running the project

```shell
pip install -r requirements.txt
# Install the required libraries
python main.py
# Run the main.py file
```

### Viewing, Adding, and Deleting Data in the Database

<hr>

To view the data in the database, simply send a GET request to the following URL:

```shell
http://127.0.0.1:5000/user/list
```

**Example**

![image](/images/example1.png)

<hr>

To add data to the database, send a POST request to the following URL with the data you want to add:

```shell
http://127.0.0.1:5000/user/add
```

**Example**

![image](/images/example2.png)

To view the documents in the database, send a GET request to the following URL:

```shell
http://127.0.0.1:5000/user/doclist
```

**Example**

![image](/images/example3.png)

To delete a document from the database, send a DELETE request to the following URL with the document ID:

```shell
http://127.0.0.1:5000/user/delete/<document_id>
```

**Example**

![image](/images/example4.png)

<hr>

Please note that the above URLs assume you are running the project locally on your machine. Modify the base URL accordingly if you are running the project on a different server or port.
