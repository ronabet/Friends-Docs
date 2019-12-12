---
id: doc4
title: API Routes
---

## Getting Started

>First of all, Thank you for using our project! for any requests or ideas for making this documentation better, please contact us for making this docs the best for your usage!

<!-- ## Friends Client Website Tutorial -->

#### Friends Client Website

[https://51.144.178.121](https://51.144.178.121)

## Response Structure
Type: ```GET``` <br>
Route: ```/api/createGroup```<br>
Example for JSON to send for API:

```json{
 "name": "checkingCreteWotjoutAdmin14437654",
 "people": [{
    "user": {
    "_id": "5d2594e36fcb691a0d178a71",
    "hierarchy": [
        "aman",
        "sapir"
    ],
    "fullName": "first",
    "personalNumber": "111111",
    "secondaryDomainUsers": [{
        "adfsUID": "first@fgh",
        "uniqueID": "first@fgh.idf"
    },
    {
        "adfsUID": "first@qwe",
        "uniqueID": "first@qwe.idf"
    }],
    "mail": "first@test.com"
    },
    "admin": false
},
    {
    "user": {
    "_id": "5d9b57b9d8c49cc66964b1f6",
    "hierarchy": [
        "כובעי הקש"
    ],
    "fullName": "ליברמן כבר",
    "personalNumber": "0099908",
    "secondaryDomainUsers": [
    {
        "adfsUID": "nitro@jello.com",
        "uniqueID": "nitro@jellouid"
    }
    ],
        "mail": "t23456789@jello.com"
    },
        "admin": true
    }
    ],
    "imgPath": "assets/img/default3.png",
    "description": "חחחחחחחחח"
}
```


Type: ```POST``` <br>
Route: ```/api/sendEmail```<br>
Description: Mail sender for all members in group. <br>
Example for JSON to send for API:
```json
{
	"groupId": "5d46a9c76533f31bb00a962z",
	"subject": "hahaha",
	"text": "hihihih"
}
```

Type:  ```PUT``` <br>
Route: ```/api/updateGroup```<br>
Description: Update all parameters of group.<br>
Parameters: Group ID from Mongo.<br>
Example for JSON to send for API: Like the request "Create group".<br>


Type: ```GET``` <br>
Route: ```/api/getAllGroups```<br>
Description: Returns all groups from the DB. <br>

Type: ```GET``` <br>
Route: ```/api/allGroups/getGroupsByPerson/:namePerson```<br>
Description: Returns all groups that user member/admin them.<br>
Parameters: Name of user.<br>

Type: ```GET``` <br>
Route: ```/api/allGroups/getGroupsByPersonAdmin/:id```<br>
Description: Returns all groups that user member them.<br>
Parameters: ID of user from MongoDB.<br>

Type: ```GET``` <br>
Route: ```/api/allGroups/getGroupsByPersonAdmin/:id```<br>
Description: Returns all groups the user is admin labeled.<br>
Parameters: User ID from Mongo.<br>

Type: ```GET``` <br>
Route: ```/api/allGroups/getGroupsByPersonNotAdmin/:id```<br>
Description: Returns all groups the user is only member, not admin.<br>
Parameters: User ID from Mongo.<br>

Type:  ```GET``` <br>
Route: ```/api/getOneGroupById/:id```<br>
Description: Returns group details by ID.<br>
Parameters: Group ID from Mongo.<br>

Type:  ```GET``` <br>
Route: ```/api/getOneGroupByName/:name```<br>
Description: Returns group details by fullname.<br>
Parameters: FullName of group.<br>

Type:  ```GET``` <br>
Route: ```/api/getAllGroupBySymbols/:name```<br>
Description: Returns all groups that has chars from the request in the fullname.<br>

Type:  ```GET``` <br>
Route: ```/api/getAllGroupMembersByID/:id```<br>
Description: Returns all members of group by ID.<br>
Parameters: Group ID from Mongo.<br>

























