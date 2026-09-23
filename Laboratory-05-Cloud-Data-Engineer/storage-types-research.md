# Types of Cloud Storage

| Storage Type   | Description                                                                              | Primary Use Case                                                                   | Cloud Provider Example |
| -------------- | ---------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------- |
| Block Storage  | Stores data in fixed-size blocks that can be accessed separately.                        | Best for virtual machines, databases, and applications that need fast storage.     | AWS EBS                |
| File Storage   | Stores data as files in folders and allows multiple users or systems to access them.     | Best for shared files, documents, and applications that need a shared file system. | AWS EFS                |
| Object Storage | Stores data as objects together with information about the data and a unique identifier. | Best for large amounts of unstructured data such as images, videos, and backups.   | AWS S3                 |

Object Storage is the best choice for the client's user uploaded images because it is designed to store large amounts of unstructured data. It can also make the images easier to access and manage as the photo-sharing application grows.

