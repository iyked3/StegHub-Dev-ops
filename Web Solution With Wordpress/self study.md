# What is a web solution?

A web solution is a comprehensive and integrated approach to address all aspects of a web project or problem. It takes into account all technical, functional, and business requirements to deliver a finished product or service that is fit for purpose and meets the needs of the customer or client. A web solution may include web development, web design, web content management, eCommerce, web hosting, web security, and more.  An effective web solution will take into account the specific needs of the customer or client, and deliver a finished product or service that meets those needs. It will be fit for purpose and provide value for money. A web solution should also be scalable so that it can grow and adapt as the needs of the customer or client chan


## Wordpress

WordPress (also known as WP or WordPress.org) is a web content management system. It was originally created as a tool to publish blogs but has evolved to support publishing other web content, including more traditional websites, mailing lists and Internet forum, media galleries, membership sites, learning management systems and online stores. Available as free and open-source software, WordPress is among the most popular content management systems – it was used by 43.1% of the top 10 million websites as of December 2023.  WordPress is written in the PHP language and paired with a MySQL or MariaDB database. Features include a plugin architecture and a template system, referred to within WordPress as "Themes".
To function, WordPress has to be installed on a web server, either as part of an Internet hosting service or on a computer running the WordPress software package.

## PHP 

PHP is a general-purpose scripting language geared towards web development. PHP was originally an abbreviation of Personal Home Page, but it now stands for the recursive initialism PHP: Hypertext Preprocessor. PHP code is usually processed on a web server by a PHP interpreter implemented as a module, a daemon or a Common Gateway Interface (CGI) executable. On a web server, the result of the interpreted and executed PHP code—which may be any type of data, such as generated HTML or binary image data—would form the whole or part of an HTTP response. Various web template systems, web content management systems, and web frameworks exist that can be employed to orchestrate or facilitate the generation of that response. Additionally, PHP can be used for many programming tasks outside the web context, such as standalone graphical applications and drone control. PHP code can also be directly executed from the command line.

## MySQL

MySQL is an open-source relational database management system (RDBMS).  A relational database organizes data into one or more data tables in which data may be related to each other; these relations help structure the data. SQL is a language that programmers use to create, modify and extract data from the relational database, as well as control user access to the database. In addition to relational databases and SQL, an RDBMS like MySQL works with an operating system to implement a relational database in a computer's storage system, manages users, allows for network access and facilitates testing database integrity and creation of backups.MySQL has stand-alone clients that allow users to interact directly with a MySQL database using SQL, but more often, MySQL is used with other programs to implement applications that need relational database capability. MySQL is a component of the LAMP web application software stack (and others), which is an acronym for Linux, Apache, MySQL, Perl/PHP/Python. MySQL is used by many database-driven web applications, including Drupal, Joomla, phpBB, and WordPress.

## MariaDB

MariaDB is a community-developed, commercially supported fork of the MySQL relational database management system (RDBMS), intended to remain free and open-source software under the GNU General Public License. MariaDB is intended to maintain high compatibility with MySQL, with exact matching with MySQL APIs and commands, allowing it in many cases to function as a drop-in replacement for MySQL. However, new features are diverging.[6] It includes new storage engines like Aria, ColumnStore, and MyRocks.

## Understanding Three-Tier Architecture

A Three-Tier Architecture is a client-server architecture model that separates an application into three interconnected but distinct layers, each responsible for specific aspects of the application's functionality.

![3 tier](images/tier.png)

#### Generally, web or mobile solutions are implemented based on a Three-Tier Architecture to improve scalability and flexibility. The three distinct layers are:

1. Presentation Layer (PL): This is the user interface such as the client server or browser on your laptop.

2. Business Layer (BL): This is the backend program that implements business logic (i.e. Application or Web Server).

3. Data Access or Management Layer (DAL): This is the layer for computer data storage and data access (i.e. Database Server or File System Server such as FTP Server or NFS Server).

## What is Logical Volume Manager (LVM)?

![LVM](images/lvm.jpeg)

LVM stands for Logical Volume Manager, a technology used in Linux and other Unix-like operating systems to manage storage devices and create flexible, resizable storage configurations. LVM provides a layer of abstraction between the physical storage devices (such as hard drives, SSDs, or partitions) and the file systems or logical volumes used by the operating system.

Key components of LVM include:

1. Physical Volumes (PVs): These are the physical storage devices or partitions (i.e. hard drives or SSDs) that are added to the LVM system.

2. Volume Groups (VGs): Volume Groups are created by combining one or more Physical Volumes. VGs serve as a pool of storage that can be allocated to various Logical Volumes.

3. Logical Volumes (LVs): Logical Volumes are similar to traditional partitions and are created within a Volume Group. They are what you format with a file system and use to store data. Logical Volumes can be resized and moved dynamically, which is a significant advantage of LVM.

## How To Implement a WordPress Website with LVM Storage Management

The following steps are taken to implement a WordPress Website with LVM Storage Management:

Step 1: Provision a Web Server EC2 Instance

1. Name of Instance: Web Server
2. AMI: Red Hat Enterprise Linux 9 (HVM), SSD Volume Type
3. New Key Pair Name: web11
4. Key Pair Type: RSA
5. Private Key File Format: .pem
6. New Security Group: WordPress
7. Inbound Rules: Allow Traffic From Anywhere On Port 80 and Port 22.

Step 2: Provision a Database Server EC2 Instance

Use the following parameters when configuring the EC2 Instance:

1. Name of Instance: Database Server
2. AMI: Red Hat Enterprise Linux 9 (HVM), SSD Volume Type
3. Key Pair Name: web11
4. New Security Group: WordPress
5. Inbound Rules: Allow Traffic From Anywhere On Port 22 and Traffic from the Private IPv4 address of the Web Server on Port 3306 (i.e. MySQL).