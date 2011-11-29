Clustered-Jackrabbit Configuration Example

* Required:
	* [Apache Tomcat 6.0.x](http://tomcat.apache.org/download-60.cgi)
	* [PostgreSQL 8.4 or higher](http://www.postgresql.org/download/)
	* [Jackrabbit binary Libraries 2.2.x](http://jackrabbit.apache.org/downloads.html)

Please refer to my [blog post](http://greymeister.blogspot.com/2011/11/jackrabbit-clustering-primer.html) for more information.  Here is a brief summary of the contents:

* repository
	* repository.xml > Sample configuration file for the clustered repository
* tomcat
	* conf
		* server.xml > Contains the GlobalNamingResources for the JDBC Datasource used by JCR
		* context.xml > Contains the JNDI resource for the JCR
	* lib
		* jars.to.include.txt > Outlines the jar files needed for Tomcat to load JCR as a JNDI resource