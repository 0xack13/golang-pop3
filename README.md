POP3 Server written in Go
=========================
This is a very simple POP3 server written in Go. My goal was to develop a simple POP3 server that can be used for further developing.

Also check out an SMTP server powered by NodeJS, that can be used together with this project!
https://github.com/r0stig/basic-smtpserver

Follow me in Twitter:
> r0stig


Installation:

```
go get ./...
```

Run the pop3 server:
```
go run main.go database.go
```

Start mongodb server in a container:
```
docker run -d -p 27017-27019:27017-27019 --name mongodb mongo:4.0.4
docker exec -it 4608 bash
mongo
use robmail
db.users.insert({username:"test", password:"password", messages: [{header:"dummy header", message: "dummy message", subject:"dummy subject"}]})
```
