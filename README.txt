# Job Connect

### Description
Job Connect is a software that helps connect between applicant and recruiter

### Installations
- [MongoDB Compass](https://www.mongodb.com/try/download/community) 
- [Database tools](https://www.mongodb.com/docs/database-tools/) (Remember see [installation guide](https://www.mongodb.com/docs/database-tools/installation/installation/))
- IDE or Editor JS (Ex: [VSCode](https://code.visualstudio.com/download))

### Import database
1. Open MongoDB Compass, click Connect to create a connection (copy your connection string)
2. Create a database "jobconnect":
    - Can use GUI
    - Or type this command into _MONGOSH (bottom in the screen):
    `use jobconnect`
3. Then, open CLI 
    - Navigate to project `cd <path to project>`
    - Type: 
    `mongorestore --db=jobconnect dump/jobconnect/ --uri="<your connection string>"`
    - Data in mongodb will be showed

DB Tool details: [here](https://www.mongodb.com/docs/database-tools/mongodump/#std-label-mongodump-examples)
- Export: `mongoexport --collection=user --db=jobconnect mongodb://localhost:27017`
- Import: 
```
mongoimport --db=jobconnect --type=json --uri="mongodb://localhost:27017" --jsonArray users.json recruitments.json companies.json
```

### Running project
1. Open terminal and navigate to project
2. Type: `node app.js`

### Accounts
- Applicant: luuduchai / 32ut2lPw3me&i
- Recruiter: admin / 1234

### Authors
- Lưu Đức Hải
- Nguyễn Hữu Đức
- Ngô Hoàng Khôi
- Lê Sỹ Tiến