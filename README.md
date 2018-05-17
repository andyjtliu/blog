# blog
steps to run the simple blog system

1) python, web.py available on server. 
2) DB mysql was available, with DB name, user, password separately "db01", "dbu1" and "123456". If it is not mysql, DB connection statement in "/DbOpr.py" should be changed accordingly, that is to change "db = web.database(dbn = 'mysql', db = 'db01', user = 'dbu1', pw = '123456')".
3) source files (especially for postfix py and html) should be put in below structure. The DDL files are just for one-off execution to create tables.
files
/blog.py
/DbOpr.py
/templates:
    /templates/base.html
    /templates/edit.html
    /templates/index.html
    /templates/index_follow.html
    /templates/index_follow_post.html
    /templates/index_self_post.html
    /templates/new.html
    /templates/register.html
    /templates/view.html
/entries.ddl
/follow.ddl
/users.ddl
4) run the project with command "python blog.py"
5) access the system through http://localhost:8080/ or througg http://<-ip->:8080

