# Premise

In one development team, we wanted to create a list of TODO comment that was written in the source code, I made a command-line tool.

This tool searches the comment, including the "TODO" from the package of the specified Go, is intended to be displayed on the standard output.

[![https://gyazo.com/9ba6056b6fa83fbbc6ad987a0131f10f](https://i.gyazo.com/9ba6056b6fa83fbbc6ad987a0131f10f.png)](https://gyazo.com/9ba6056b6fa83fbbc6ad987a0131f10f)

For example, you can search for TODO comments fmt package as follows.

The source code for this tool, please refer to the main.go that have been attached.

It should be noted, main.go that is attached operates in Go1.7 more.

# Task
In this team, we wanted the above tools and extended as follows.

1. I want to be able to change the search string (such as "TODO" or "FIXME")
2. I want to work with Go1.6.2 more
3. I want to also provide server mode
4. If you start as a server mode, it operates as an API server
5. Sending a HTTP request with a string to search for the package import path (such as fmt and net / http) to the server, come back the results in JSON format
6. At least in the response, which contains the corresponding file path, row, the target comment

So as to satisfy the above requirements, please correct the main.go.

It should be noted that the format of the response and request of the API does not matter if I have freely design.

It does not need to fit in a single package or a single file.

There is no need to comply with the writing of the appended to have main.go, it does not matter if I have freely improved.

In addition, we ask you to please answer the following in mind:.

- Premise that this tool has been maintained in the team
- It is actively improvement that can be improved in the existing code
- Attach a code that operation can be verified
- API documentation can be generated from the source code who created
