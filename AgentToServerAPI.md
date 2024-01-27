# API Documentation

## Agent - API REST

### Request

#### Method

 - `GET` for the first request (on agent restart)
 - `POST` for other requests with orders results

#### URL

http://webscripts.server/c2/order/[agent_random_key_and_identifier]

#### Headers

The `User-Agent` should be `Agent-C2-EX-MACHINA X.X.X (System) hostname` (where `X.X.X` is the version and subversions, `System` is `Windows`, `Linux` or `Darwin` and `hostname` is the server name).

#### Format

```json
{
    "NextRequestTime": int,
    "Tasks": [
        {
            "Type": "TYPE",
            "User": "USERNAME",
            "Name": "TASKNAME",
            "Description": "TASK_DESCRITPION",
            "Data": "DATA",
            "Filename": "FILENAME OR LAUNCHER",
            "Timestamp": int,
            "Timeout": int,
            "Id": int,
            "After": int
        },
        {
            "Type": "TYPE",
            "User": "USERNAME",
            "Name": "TASKNAME",
            "Description": "TASK_DESCRITPION",
            "Data": "DATA",
            "Filename": "FILENAME OR LAUNCHER",
            "Timestamp": int,
            "Timeout": int,
            "Id": int,
            "After": int
        }
    ]
}
```

##### NextRequestTime

Next request unix epoch timestamp.

##### Tasks

###### Type 

Type define sent data type, such as : "COMMAND"

```
COMMAND       =    execute content of data field
UPLOAD        =    upload file from server to agent
DOWNLOAD      =    download file from agent to server
TEMPSCRIPT    =    upload a script in a temp file, execute it and remove the temp file
MEMORYSCRIPT  =    Execute the script in memory (as argument)
```

###### User

User name who as launched the task, to log/store on the agent system. This information can be useful for forensic or investigation.

###### Name

Task name to log/store on the agent system. This information can be useful for forensic or investigation.

###### Description

Task description to log/store on the agent system. This information can be useful for forensic or investigation.

###### Data 

Data define the content of the order to execute or source and destination to download/upload file.

###### Filename

Laucher for `SCRIPT` and `MEMORYSCRIPT` (`powershell`, `python3`, `python2`, `python`, `perl`, `bash`, `shell`, `batch`, `vbscript`, `jscript`) and filename for `UPLOAD`.

###### Timestamp 

Unix epoch timestamp define the exact time stamp when the order should be executed

###### Timeout

Maximum time (in seconds) to execute the task.

###### Id

Order Id

###### After

Order Id or `null`, to execute this order after any precedent order (use case: an order is a requirement for another order).

### Response

#### Format

```json
{
    "Tasks": [
        {
            "Id": int,
            "Stdout": "<output content>",
            "Stderr": "<error messages>",
            "Status": int,
            "StartTime": int,
            "EndTime": int
        }
    ]
}
```

##### Id

The task ID sent by the the server in the responses.

##### Stdout

The output content for the executed task (for example on command order this is the command standard output).

##### Stderr

Any error message should be here, that include logs.

##### Status

The status should be `0` if task end without any error else status should be greater than `0` (on command task this is the command exit code).

## Malware
