# Persistance Layer
This is the branch for all the persistence-layer atomics that can create and maintain the physical data store. 
We use relational and document-oriented datastores that contain the data and metadata needed to drive the metaverse reality, serving as our DataBase of Record (DBoR). Thus, yes, **our database is multiversal database**. 
## Implementation Choices
At this time we choose the opensource **MySQL** as the relational database engine. This is the main engine. 
At this time we choose the opensource **MongoDB** as the document-oriented database engine. 
## Input/Output formats
Input/output formats include **sql, xml, blend, text, and xls** files that can be read/written
## Use Case
The idea is that a content creator can register as a content creator, create a .blend file on their PC, and SFTP (upload for you dweebs) it to a folder on the metaverse site. The site will detect the file, import it into the metaverse. and email the creator. Inside the blend file is metadata that indicate its version, creator, license, economy, dependencies/inheritances, and universe(s) it is to be included in, as well as content describing the actual object itself (scenes, points, textures, animations, etc.). After processing the file and updating the relevant DBoRs, the presentation systems will be notified to update and show this new object in its place (when in view and matching conditions!) 
## What's Next?
For the relational databases, you will find a set of SQL files that establish each database schema and then individual SQL files to create/update the individual tables. Consult the **readme.sql** file for a sequential list of SQL files to run in order to keep your schema up to date. 
