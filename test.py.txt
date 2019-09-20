#! /usr/bin/env python

import mysql.connector
mydb = mysql.connector.connect(host="mysql1", user="root", passwd="password", auth_plugin="mysql_native_password")

testCursor=mydb.cursor()
testCursor.execute("create database studentdb")
testCursor.execute("show databases")

for x in testcursor:
        print(x)
