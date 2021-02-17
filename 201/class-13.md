# Class 13 Reading
# THE PAST, PRESENT & FUTURE OF LOCAL STORAGE FOR WEB APPLICATIONS
- when we use any web browsre we see that we can store and retrive data.
- in web browsre there is camething called cookies (in other language called log file).
- this cookies(log file) it store the user data the browse the web page and it store in file we name it registry file.
- the registry file have multiple type:
    1. INI files
    2. XML files
    3. etc....
- the cookies have small amount of storge to small amount of data.
- the cookies included in every HTTP request.
- there is some drawback for cookies:
    1. make your web application slowlly
    2. it send data without encrypted it 
    3. limited space for data 4kb.

# A BRIEF HISTORY OF LOCAL STORAGE HACKS BEFORE HTML5
- ther was defferent companies that have the compitition to create browsers
- Microsoft invented Internet Explorer and  many things one of these thing was called DHTML behaviors
- userData one of thies behaviors that allow the wep pages to store data up to 64KB of data per domain
- in 2002 adobe invented Flash 6 and give it some feature .
- one of theis feature known as Local Shared Objects it allow to store up to 100KB of data per domain
- in 2007 Google launched Gears to provide more space to store data.


# INTRODUCING HTML5 STORAGE
- when  HTML5 Storage it take the storge to another level
- we can use this name to refer HTML5 Storage Local Storage or DOM Storage.
- the way that HTML5 use to store data is pair key\value .
- the data that will create it never transmitted  to server 


# USING HTML5 STORAGE
- beacuase we store data in HTML5 as pairs key\value we can use the same the same key to retrive the value
- JavaScript supported any type of data the stored in HTML5 storage

# TRACKING CHANGES TO THE HTML5 STORAGE AREA
- we can track the storage data by using the storage event.
- storage event is supported in all browsers
- storage event can't be canceled 

# LIMITATIONS IN CURRENT BROWSERS
- in HTML5 the default limit of storage is 5MB if we store data large than 5MB it will occur an error we call it QUOTA_EXCEEDED_ERR

# HTML5 STORAGE IN ACTION
- there is a good thing in HTML5 storage that it will save your data in the browsre even when you close it 


# BEYOND NAMED KEY-VALUE PAIRS: COMPETING VISIONS
- Google provide new Storage type called SQLite that provide us more space to store our data 
- there is multiple version of sql:
    1. Oracle’s SQL
    2.  Microsoft’s SQL
    3. MySQL’s SQL
    4.  PostgreSQL’s SQL
    5. SQLite’s SQL