## What Is Network-attached storage (NAS)
![alt text](images/nfs.png)

Network-attached storage (NAS) is a file-based storage architecture that makes stored data more accessible to networked devices means multiple users or client devices retrieve data from a single storage system. As the multiple clients or users connected through a Local Area Network access the data from a centralized disk capacity by Ethernet that’s why it is referred to as Network Attached Storage. Network Attached Storage(NAS) gives all the connected devices of the network a single access point for storage which is called NAS Storage Server. 

* NAS Hardware: A NAS box, NAS unit, NAS server, or NAS head is an example of network appliance hardware (NAS) and is essentially just a server with CPUs, Random Access Memory (RAM), and storage devices..
*  NAS Software: Storage software is installed in the dedicated hardware of the NAS hardware system. NAS software is deployed on a lightweight Operating System. 
*  NAS Protocol: Data transfer protocols are there for sending and receiving data that are accessed by switches. Internet Protocol(IP) and Transfer Control Protocol(TCP) is the most fundamental data transfer protocol that is there through most clients/users transfer data.
  
### What is Network Attached Storage Used for?
 
* For storing and exchanging files.
* For data backup and catastrophe recovery, create active data archives.
* Provide a virtual desktop environment.
* Test and create server-side and web apps.
* Stream torrents and media files
*Save any pictures and movies that you need to access frequently.
* Establish a printing repository within the company.

### Components of NAS
* Processor: Every NAS has a processor at its core, which monitor the memory and central processing unit (CPU).
* Interface of a network: USB and Wi-Fi connectivity are two examples of direct computer connections that small Network Storage Devices (NAS) intended for desktop or single-user use may support.
* Physical storage: It usually takes the form of disc drives, is a requirement for every NAS. The drives, which frequently accommodate a variety of various storage devices, may be conventional magnetic HDDs, SSDs, or other non-volatile memory devices.
* Operating System: The OS arranges and controls the NAS hardware and makes storage accessible to clients, such as users and other apps, much like it does on a traditional computer.

### Advantages of NAS
* Performance – Provides better performance in serving files.
*High-end data features – Provides storage management and security.
* Scale-up – Supports a scalable storage system.
* Accessibility – Every client/user in the network can easily access to NAS.
* Easy setup – NAS architecture is easy to set up.

Disadvantages of NAS

* Complexity: A SAN can increase workload management by adding new layers of complexity to already-existing systems.
* Cost: For new users, the expense of setting up and maintaining a SAN may be prohibitive.
* Management: SANs can be difficult to oversee and may need to be managed by a specialised professional.


## Storage Area Networks

![alt text](images/san.jpg)

A dedicated, fast network that gives storage devices network access is called a Storage Area Network (SAN). SANs are generally made up of several technologies, topologies, and protocols that are used to connect hosts, switches, storage elements, and storage devices. SANs can cover several locations.

Data transfer between the server and storage device is the primary goal of SAN. Additionally, it makes data transmission across storage systems possible. Storage area networks are primarily used to connect servers to storage devices including disk-based storage and tape libraries.

### Types of Storage Area Networks

* Fibre Channel (FC): A Fibre Channel is one of the maximum broadly used SAN storage connections. It presents excessive-velocity, low-latency connectivity between servers and storage devices with the use of fibre optic cables. Fibre Channel helps factor-to-factor, arbitrated loop, and switched fabric topologies. It gives excessive throughput, reliability, and scalability, making it suitable for traumatic enterprise environments.

* Internet Small Computer System Interface(iSCSI): iSCSI is a storage protocol that transmits SCSI commands over TCP/IP networks, permitting servers to get the right of entry to faraway storage devices using fashionable Ethernet connections. ISCSI offers a value-effective alternative to Fibre Channel, leveraging current Ethernet infrastructure and TCP/IP networks. It presents features such as block-level garage access, multipathing, and CHAP authentication.

* NVMe over Fabrics (NVMe-oF): NVMe over Fabrics extends the NVMe garage protocol over excessive-pace networks, together with Ethernet or Fibre Channel, to offer low latency.

* Fibre Channel over Ethernet (FCoE): Fibre Channel over Ethernet encapsulates Fibre Channel frames into Ethernet packets, allowing Fibre Channel site visitors to be transmitted over Ethernet networks. FCoE enables the convergence of storage and data networks, lowering infrastructure complexity and fees. It leverages Ethernet’s sizable adoption and familiarity at the same time as preserving Fibre Channel’s overall performance characteristics.

* Serial Attached SCSI(SAS): Serial Attached SCSI is a factor-to-point garage protocol designed to attach servers to garage gadgets using high-pace serial connections. SAS gives overall performance akin to Fibre Channel but with less difficult cabling and decrease expenses. It helps direct-connected garage (DAS) and may be used in SAN environments with SAS switches or routers.

### Advantages of SANs

* Increased accessibility of applications.
Storage is available through numerous pathways for improved dependability, availability, and serviceability and exists independently of applications.

* Improved functionality of the programme
Storage Area Networks (SANs) transfer storage processing from servers to different networks.

* High availability, scalability, flexibility, and easier management are all made feasible by central and consolidated SANs.

* By using a remote copy, remote site data transfer and vaulting SANs shield data from malicious assaults and natural disasters.

* Straightforward centralised administration
SANs make management easier by assembling storage media into single images.


Disadvantages of SANs

* If client PCs require high-volume data transfer, SAN is not the best option. Low data flow is a good fit for SAN.

* More costly.

* It is quite challenging to keep up.

* Sensitive data may leak since every client computer has the same set of storage devices. It is best to avoid storing private data on this network.

* A performance bottleneck is the result of poor implementation.

* Maintaining a data backup in the event of a system failure is challenging.

* Too costly for small businesses
need a highly skilled individual

## What is NFS (Network File System)?
![alt text](images/nfs%20architecture.jpg)
NFS, or Network File System, was designed in 1984 by Sun Microsystems. This distributed file system protocol allows a user on a client computer to access files over a network in the same way they would access a local storage file. Because it is an open standard, anyone can implement the protocol. NFS started in-system as an experiment but the second version was publicly released after the initial success.

### How does NFS work?

To access data stored on another machine (i.e. a server) the server would implement NFS daemon processes to make data available to clients. The server administrator determines what to make available and ensures it can recognize validated clients.

From the client's side, the machine requests access to exported data, typically by issuing a mount command. If successful, the client machine can then view and interact with the file systems within the decided parameters

## What is SFTP?
![alt text](images/sftp.jpeg)

SFTP is similar to FTPS in that it uses AES and other algorithms to secure data as it travels between different systems. SFTP also provides several methods to fulfill the authentication of a connection such as user IDs and passwords, SSH keys, or combinations of these. SFTP is capable of helping enterprises achieve file transfer compliance as required for HIPAA, GDPR, and other regulatory regimes.

Compared to other file transfer protocols such as FTPS, SFTP may offer an advantage, particularly when it comes to authentication over firewalls . In this sense, SFTP offers less risk than FTPS, since it only requires a single open port to send and receive initial authentication information, commands, and file transfers from another server. 

Another advantage of SFTP is that it is packet-based instead of text-based. What this means is that SFTP is typically faster than other file transfer protocols since packets are easier to process, hence requiring fewer CPU resources. Whereas text-based protocols can contain large strings that take substantially more time to decrypt. In other words, SFTP is easier to process simply because less data is changing hands. 


## Server Message Block (SMB)
![alt text](images/smb.png)
The Server Message Block (SMB) protocol is a client-server communication protocol that is used for shared access to files, directories, printers, serial ports, and other resources on a network. It also provides an authenticated inter-process communication (IPC) mechanism.

Server Message Block (SMB) file system
Server Message Block file system (SMBFS) allows access to shares on SMB servers as local file systems in the AIX® operating system by using SMB protocol version 1.0.
Server Message Block (SMB) client file system
The SMB client file system is based on the SMB protocol version 2.1 and version 3.0.2. You can use the SMB client file system to access files on an SMB server.

## What is iSCSI?
![alt text](images/iscsi.jpg)

The SNIA dictionary defines iSCSI (Internet Small Computer Systems Interface) as a transport protocol that provides for the SCSI block protocol to be carried over a TCP-based IP network, standardized by the Internet Engineering Task Force and described in RFC  7143 and RFC 7144.

iSCSI, like Fibre Channel, can be used to create a Storage Area Network (SAN). iSCSI traffic can be run over a shared network or a network dedicated to storage. However, iSCSI does not support file access Network Attached Storage (NAS) or object storage access (they use different transport protocols).

There are multiple transports that can be used for iSCSI. The most common is TCP/IP over Ethernet, but Remote Direct Memory Access (RDMA) can also be used with iSER, which is iSCSI Extensions for RDMA. If using iSER, the transport is RoCE or InfiniBand and the underlying network is Ethernet (for RoCE) or InfiniBand (for InfiniBand transport).

iSCSI is supported by all major operating systems and hypervisors and can run on standard network cards or specialized network cards (see TOE below). It is also supported by almost all enterprise storage arrays. For these reasons it has been popular for so-called “Tier 2” applications that require good, but not the best, block storage performance, and for storage that is shared by many hosts. It also is very popular among hyperscalers and large cloud service providers when they need a block storage solution that runs over Ethernet.


## What is block storage?

Block storage is technology that controls data storage and storage devices. It takes any data, like a file or database entry, and divides it into blocks of equal sizes. The block storage system then stores the data block on underlying physical storage in a manner that is optimized for fast access and retrieval. Developers prefer block storage for applications that require efficient, fast, and reliable data access. Think of block storage as a more direct pipeline to the data. By contrast, file storage has an extra layer consisting of a file system (NFS, SMB) to process before accessing the data.

### What are the benefits of block storage?
##### Organizations use block level storage because of the following advantages.

#### Performance

Metadata is additional data that describes the primary data contained in the storage system. Block storage uses limited metadata but relies on unique identifiers assigned to each block for read/write operations. This reduces data transfer overhead and allows the server to efficiently access and retrieve data in block storage. Because block storage metadata is limited, block storage delivers ultra-low latency required for high-performance workloads. This is required for latency sensitive applications like databases. For example, Viasat uses Amazon Elastic Block Store (Amazon EBS) to capture high throughput (highly transactional) data and optimize storage costs. Organizations use Amazon EBS for performance and cost optimization, scale and agility, and for data protection with EBS Snapshots.

#### Flexibility and scalability

Block storage devices are not constrained to specific network environments. Individual blocks can be configured for different operating systems, such as Windows or Linux. Developers can share data across multiple environments to ensure high availability. The block storage architecture is also highly scalable. Developers can add new blocks to existing ones to meet growing capacity needs.

#### Frequent modification
Block storage supports frequent data writes without affecting performance. Instead of rewriting the entire file, the system identifies the particular block that needs to be amended. Then, it rewrites the selected block with the new data. This makes block storage very efficient for managing large files that require frequent updates.

#### Granular control
Developers gain a high degree of control over storing data on block storage. For example, they can optimize performance by grouping fast-changing data on specific blocks and storing static files on others. This improves system performance as ongoing updates only affect a small number of data blocks instead of an entire file. For example, block storage gives you the flexibility to tier fast-changing data on solid state disk (SSD) for the highest performance, and store warm or cold data on lower cost hard drives (HDD).

### Object storage

Object storage is a technology that stores and manages data in an unstructured format called objects. Each object is tagged with a unique identifier and contains metadata that describes the underlying content. For example, object storage for photos contains metadata regarding the photographer, resolution, format, and creation time.

Developers use object storage to store unstructured data, such as text, video, and images. 

## Block storage compared to object storage
![alt text](images/bof.png)
Both storage solutions are beneficial depending on the use case. Block storage provides low latency and high-performance values in various use cases. Its features are primarily useful for structured database storage, VM file system volumes, and high volumes of read and write loads.

Object storage is best used for large amounts of unstructured data, especially when durability, unlimited storage, scalability, and complex metadata management are relevant factors for overall performance.