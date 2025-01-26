# BuildSmartDB

BuildSmartDB is a distributed database system designed to manage real-time energy usage data in smart buildings. The system employs advanced fragmentation and replication strategies to ensure high performance, scalability, and fault tolerance, making it capable of handling large-scale data inputs efficiently.

## Features

- **Distributed Data Storage**: Data is fragmented and distributed across multiple nodes, ensuring efficient storage and fast access.
- **Fault Tolerance**: Replication strategies ensure data availability and integrity, even in the case of node failures.
- **Scalability**: The system can scale horizontally, allowing it to handle increasing amounts of data without performance degradation.
- **High Performance**: Optimized for handling real-time energy usage metrics, ensuring fast query responses even with large datasets.
- **Data Integrity**: Ensures consistency across replicas and resolves issues with data distribution for optimal performance.

## Technologies Used

- **Backend**: Python
- **Databases**: PostgreSQL (Relational), MongoDB (NoSQL)
- **Architecture**: Distributed Database with Fragmentation and Replication
- **Libraries**: Custom data fragmentation and replication algorithms

## How It Works

1. **Fragmentation**: The data is divided into smaller, manageable pieces (fragments) and distributed across multiple database nodes. This improves access speed and ensures that no single node is overloaded.
2. **Replication**: The data fragments are replicated across multiple nodes to ensure high availability. In case of a node failure, the system can continue to operate by using the replicated data from other nodes.
3. **Querying**: The system supports efficient querying by distributing data fragments and ensuring that queries can be executed quickly even as the system scales.
4. **Fault Tolerance**: The system ensures that even if a node fails, no data is lost, and the system continues to function normally, allowing for seamless operation.

## Setup Instructions

### Prerequisites

- Python (v3.x or higher)
- PostgreSQL (for relational data storage)
- MongoDB (for NoSQL storage)
- Docker (for containerization, optional)

### Steps

1. **Clone the repository**

   ```bash
   git clone https://github.com/hacKRD0/BuildSmartDB.git
   cd BuildSmartDB
