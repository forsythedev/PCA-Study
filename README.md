# PCA-Study Guide

This is a study guide for the 2025 Professional Cloud Architect exam, offered by Google.

In this repo you will find the most covered topics on the exam and how I would teach them to someone trying to learn.


| Topic Name             | Description                                           | SubTopics              |
| ---------------------------- | ----------------------------------------------------- | --------------------- |
| [Storage](#storage) | Different methods and categories of storage in GCP     | Storage Options - Storage Types |


# Topics

## Storage
* Storage Options
  * SQL - Standard Query Language
    * _Used to communicate with and manage **relational databases**_
      * BigQuery
      * Cloud Spanner
      * Cloud SQL
  * NoSQL
    * _No SQL dbs offer flexible schemas and don't rely on diverse data models, Unlike SQL there is no universal language for NoSQL storage types._
      * BigTable
      * Firestore
      * Cloud Datastore (optional, legacy)
  * Object Storage
    * _Stores data as an object, just like in programming this means you the data has attributes and methods assigned to it_
      * Cloud Storage (Standard, Nearline, Coldline, Archive)
  * Block Storage
    * _Breaks down data into fixed sized blocks, then gives each block an identifier. This is how the information is stored. NoSQL and SQL can still be used to retrieve data from block storage._
      * Persistent Disks (HDD, SSD)
  * File Storage
    * Filestore
                ========================
* Storage Types
  * Standard
    * Easiest access
    * Highest cost
  * Nearline
    * +30 days
  * Coldline
    * +90 days
  * Archive
    * +365 days
    * Cheapest, mainly for backup
