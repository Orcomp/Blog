---
layout : post
title : ER Diagram Software
category : Software
tags :
  - Tools
---

I have spent a lot of time looking for an ER diagram application which:

- is free
- is cross platform
- has a small download size
- looks good and is easy to use
- saves files in a text format (for easy version control)

I found a lot of software that meet some of the criteria but not all... until I found [MySQL Workbench](http://dev.mysql.com/downloads/workbench/)

At first sight MySQL Workbench ticks all right boxes except the last one, because its file format (.mwb) is binary.
That is until I found out the .mwb file is really only a zip file which contains a nicely formatted xml file.

The best thing is that you can open the xml file directly with MySQL Workbench without any issues. (Just start MySQL Workbench and then navigate to the xml file.)

The only minor problem is saving the document will save the file back to a .mwb format, so you need to extract the xml file from the zip file again before committing the changes to version control.
This should not be a big issue if the file does not need to be modified too often.


NOTE: I am only using MySQL Workbench for it's ER diagram capabilities. You do not need to install or connect to a MySQL database server in order to use this tool. 
i.e. it works perfectly as a stand alone application.