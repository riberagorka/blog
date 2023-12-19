<link rel="stylesheet" href="/media/gorka/6AAC-AF7E/gorka/personal/articles/styling.css" />
---
layout: post
title: Blogging Like a Hacker
---
# TYPES OF STORAGE

## FILE STORAGE
## BLOCK STORAGE
## OBJECT STORAGE

# OBJECT STORAGE

## S3 STORAGE (Simple Storage Service)
In this case I am using a DELL's object storage which is called as DELL Elactic Cloud Storage (ECS) and it is very similar to the Amazon Web Service's s3 storage in its concept and purpose. It is designed to provide scalable, durable and highly available storage for large amounts of unstructured data as AWS's s3 object storage.

But what are the main characteristics and advantages of the object storage systems over other type of storages?

### KEY CHARACTERISTICS AND ADVANTAGES  OF OBJECT STORAGE

- **Scalability**: Object storage offers a highly scalage storage option, allowing you to easily scalate teh storage horizontally. The objects are stored in a flat hierarchy with unique identifiers, making those storages ideal for unstructured data as well as for large datasets. What means that the storage is ideal to store unstructured data? It means that these object storages are well-suited for storing data such as, images, videos, documents and backups among others.

- **Durability & Redundancy**: The object storages usually replicate and distribute the data accross multiple servers and locations, this allows to ensure high availability of the data and to protect against the data loss. Replication means that the data is copied into multiple locations, enhancing its availability and fault tolerance. Distribution means that the data stored is arranged into multiple locations (nodes) into the network.

- **Metadata & Tags**: The metadata allows to provide additional information about the content of the object, facilitating the organization of the unstructured data and the posterior searching of it. For example, metadata makes the objects searchable in an easier way. It also can be used to track versions of objects and manage their lifecycle, for example, being able to mark an object as "production" or "archive" and set automatic rules for data transition or deletion based on the available metadata. 
	One more thing regardin the metadata and that nowadays is a very important for data storage and management is the data governance. It provides a clear and traceable data lineage and ownership, being able to document the origin, the transformations of the data in its entire lifecycle.

- **Data Governance**:

### KEY CONCEPTS IN OBJECT STORAGE

#### Namespace
A **namespace** is a container or a partition inside the object storage that organizes and manages a set of objects inside of it.
#### Bucket
A **bucket** is a storage container defined by the user and it is located inside a specific namespace. A bucket server to organize and manage objects inside it.

#### Object
An **object** is the fundamental unit of data in the object storage. Each object inside a bucket is uniquely identified and includes both, the data and the metadata.

#### User
A **user** is an entity with associated credentials, which grants the user with the necessary permissions to list, read, write the object or create and delete the buckets. This credential are defined by policies, which allows the user to perform those specific actions.

#### IAM (Identity & Access Management)
**IAM** is a framework used to manage access to the resources securely. It is used for the creation and management of the users and their respective policies.

![Namespace basic structure](images/namespace-basic-structure.drawio.png)

### POLICIES & ACCESS CONTROL

A **policy** is a set of rules that define the permissions given to a certain entity in the object storage. For example, we can define a policy that grant to the user *test* to read and write objects in a certain bucket.

#### Bucket Policies

**Bucket policies** are 

#### User Policies

General idea of a namespace structure:
![Namespace structure](images/namespace-structure.drawio.png)

#### ACLs

#### Types of Restrictions

#### Zero Trust Policy

