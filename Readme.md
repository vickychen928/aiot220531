# AIoT Github

## Lecture 15: IoT Flask Web (deploy to heroku)
#### Author: Vicky Chen 


### step 0：register and download
 * 註冊Heroku, github
 * 下載HeidiSQL, VS code


### step 1 : Clone this github
* git clone https://github.com/huanchen1107/aiot0530-start-no-token 到 local\aiot220531 folder
* 把local的 \aiot220531\ .git 殺掉 (產生自己的git管理員) 方便建立新的git repository 
* 推送至github建立新的aiot220531 (https://github.com/vickychen928/aiot220531)


### step 2 : install some package
```python
pip install gunicorn Flask==2.0.1 Jinja2==3.0.1 psycopg2 sklearn pandas numpy 
```

### step 3: add an heroku postgredb
* register heroku account
* go to dashboard
* new an app
* go to resource and add-on an Heroku postgredb


### step 4: login to heroku postgredb using HeidiSQL
* 在app.py改成用heroku postgredb
```sql
myserver ="<fill-in-Heroku-Postgredb-DB-sever>"
myuser="<fill-in-Heroku-Postgredb-DB-user>"
mypassword="<fill-in-Heroku-Postgredb-DB-pwd>"
mydb="<fill-in-Heroku-Postgredb-DB-db>"
```
* 使用hedisql連接heroku postgredb
    ![](./static/hedisql.png)


### step 5: import postgredb (in db/postgre.db)




### step 6: setting db in app.py
* 將app.py中資料庫的資訊換成heroku postgredb的資訊
```sql
myserver ="<fill-in-Heroku-Postgredb-DB-sever>"
myuser="<fill-in-Heroku-Postgredb-DB-user>"
mypassword="<fill-in-Heroku-Postgredb-DB-pwd>"
mydb="<fill-in-Heroku-Postgredb-DB-db>"
```


### step 7: testing locally by running python app.py

### step 8: deploy to github (new public github repositoy 不然看不到)
delete .git and git remote add origin master github.com/xxxxx


### step 9: Heroku deploy from github

### step 10: Complete

Sample link 1:
https://awinlab-aiot.herokuapp.com/

Sample link 2: 
https://aiot0529.herokuapp.com/


![](./static/cat.jpg)


