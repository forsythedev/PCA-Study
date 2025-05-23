# PCA-Study Guide

This is a study guide for the 2025 Professional Cloud Architect exam, offered by Google.

In this repo you will find the most covered topics on the exam and how I would teach them to someone trying to learn.


| Topic Name             | Description                                           | SubTopics              |
| ---------------------------- | ----------------------------------------------------- | --------------------- |
| [Storage](#storage) | Different methods and categories of storage in GCP | [Storage Options](#storage-options) - [Storage Types](#storage-types) - [Storage Sizes](#storage-sizes)|
| [Connections](#connections) | Different ways to connect on premise, cloud based, and other GCP applications to GCP | [Connection Types](#connection-types) - [Connection Speeds](#fastest-to-slowest-connections) |


# Topics

## Storage

### Storage Options
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
======================== ======================== ======================== ======================== ========================
### Storage Types
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

======================== ======================== ======================== ======================== ========================

### Storage Sizes
   * Smallest
     * Firestore: Smallest in general, can storage even KBs
     * Cloud SQL: A few GBs or less
     * SSDs: As small as 10 GB
     * Cloud Spanner: Can work small but not meant for small
     * Big Query: Handles small data well
   * Largest
     * Tens of TB, up to 64 TB in some Google Cloud configurations
     * SSDs: As large as 64 TB
     * Cloud Spanner: Can store Petabytes of data, 1 PB is 1000 TBs
     * BigQuery: Meant for petabyte to exabyte scales of data. Best for realtime access.
     * Firestore: Scaling into petabytes gets challenging
     * BigTable: Built for peta and exabytes of data. Handles realtime access very well.
    
========================   NEXT  ========================
======================== SECTION ========================

## Connections

### Connection Types
 * Interconnects
   * Dedicated Interconnect
     * _Physical Connection between on premise network and GCP_
   * Partner Interconnect
     * _Use a supported service providers, physical connection_
   * Cross Cloud Interconnect
     * _Using another cloud services physical connection_
 * Peering
   * VPC Peering
     * _Private internal connection between two GCP VPCs_
   * Direct Peering
     * _Where your network directly connects to and exchanges information to Google. You own _
   * Carrier Peering
     * _This is when you connect to a telecommunications network that has already setup direct peering. Typically sed for accessing Google services, not VPCs. Connect with ISPs private network._
   * Private Service Connect
 * VPN
   * Cloud VPN
     * _Secure connection over the public internet._
 * Other
   * Public Internet
   * Shared VPC
   * Hybrid
  
### Fastest to Slowest Connections
* VPC Peering
* Dedicated Interconnect
* Cross Cloud Interconnect
* Partner Interconnect
* Direct Peering
* Carrier Peering
* Cloud VPN
* Public Internet
  
  
