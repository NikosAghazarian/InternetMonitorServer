# InternetMonitorServer
Tracks and stores HTTP response times from select webpages.

# Reflections
Internet Monitor:  
    -Tracks and stores HTTP response times from select webpages.  
    -Utilizes two Raspberry Pis. One to host the DB, webpage UI, and track wired connection; one to track wireless connection and send to DB.  
    -Stores time, server, response time, and connection type within a MariaDB/MySQL table.  
    -Built on the NodeJS and Express frameworks.  
    -Gives users access to the recorded information and various ways to visualize the data while on the local network via an Express app.<br/><br/>
    **Problems & Potential improvements:**  
    *Hardware:*  
    -The system could work with only one computer rather than two to track connectivity with better knowledge of networking and routing.   
    -Two solutions that seem plausible are containers with limited network interface access to force use of an interface, and use of packet marking to designate packets that should be sent to an interface.  
    *Software:*  
    -There are no glaring flaws in the software, the server doesn’t crash without targeted user effort, and the server will restart automatically.  
    -More work and time could create more ways for the user to interact with the available data, and more varied sources of data (e.g. speed testing) to be collected and aggregated for examination of network health, security, connectivity, and downtimes.  
