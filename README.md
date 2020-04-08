
# Load JSON Data into Oracle DB using Python SDK

Last Updated:<br>March 01, 2019 
</td>
<td class="td-banner">
# Load JSON Data into Oracle DB using Python SDK
</td></tr><table>

Project to load tweet data into Oracle Database deployed on Oracle Cloud Infrastructure (OCI) using Python SDK's.


## Introduction

These instructions will get you a copy of the project up and running on your local or any machine/system for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

## Prerequisites

What things you need to install the software and how to install them


- A pre-provisioned Oracle Database.


## Package Contents

* import-export
  * jsonapp.py
    * Connect to Oracle Database
    * Insert data into Oracle DB using the Python SDK.
* source
  * JSON Data 

## Components
* Data Source&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;: Twitter
* Data Collection and Processing     &nbsp; &nbsp; : Python
* Data Storage                       &nbsp;&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; : Oracle Database on Oracle Cloud Infrastructure


## Steps to Deploy

- Open terminal
- Move to the folder where you want to download the application.
- Create a directory for the application

  ```
  mkdir /pythonApp
  ```
- Move to that directory

  ```
  cd /pythonApp
  ```
- Clone the Github Repository

  ```
  git clone https://github.com/Abdul-Rafae-Mohammed/LoadDataintoOracleDBusingSDK.git
  ```
- Go inside the downloaded repository

  ```
  cd <repo name>/
  ```
  
- Open the Config File

  ```
  vi parameters.txt
  ```
- Enter the database connecition details. The data should look similar to below example:
  
- Note: Attributes in below snippet should be replaced with appropriate data for your application/database.

  ```
  jsonfile=xxxx.json
  ip=xxx.xxx.xxx.xxx
  port=xxx
  service=hxxx.xxxxxxxxx.xxxx.xxx.com
  sys_password=xxxxxx
  ```
  
- Then save the file. 

  ```
  Press Ctrl+S to save.
  ```

- Run python app

  ```
  python jsonapp.py parameters.txt
  ```

- The output should as mentioned below.

```
Database Version :  1x.x.0.0.0
User APPSCHEMA already created
Table TWEETSData already created
Tweets loaded into the database successfully!!!
```



## Authors

**Abdul Rafae Mohammed (abdul.rafae@outlook.com)**


