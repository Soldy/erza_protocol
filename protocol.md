#erza protocol for developers json 

#oauth

```javascript
/oauth2
```

#fbs

```javascript
/fbs

```

#standard get switches


```javascript

limit  | integer | 10 - 10000
offset | integer | 10 - 10000
text   | string  | varchar 10 - 1024
blob   | blob    | 1 byte 2048 kilobyte
q      | string  | varchar 1 - 48
to     | string  | short user id
from   | string  | short user id
id     | string  | short id or uuid 
sign   | string  | gpg signature

```


#get servers

## request 

```javascript
/server
```
## response

```javascript

{
   id:"", // packet id
   servers:[
       {
            id:"", // string
            name:"", // string
            uptiime:0, //integer
            rooms:0, //integer
            users:0, //integer
            endpoints:[ .// list of ips  ip:port
                  "ip:port"
            ],
            type:0 // bitwise
       }

   ],
   timestamp: 0,
   signatura:"" //string
}

```

#get rooms

## request

```javascript
/rooms
```
## response

```javascript

{
   id:"", // packet id
   rooms:[
       {
            id:"", // string
            name:"", // string
            title:"", // string
            uptiime:0, //integer
            users:0, //integer
            type:0 // bitwise
       }

   ],
   timestamp: 0,
   signatura:"" //string
}

```


#get users

## request

```javascript
/users

```
## response

```javascript

{
   id:"", // packet id
   users:[
       {
            id:"", // string
            name:"", // string
            status:0, // bitwise
            type:0 // bitwise
       }

   ],
   timestamp: 0,
   signatura:"" //string
}

```


#get messages

## request

```javascript
/messages
```

## response

```javascript

{
   id:"", // packet id
   messages:[
       {
            id:"", // string
            type:0 // bitwise
            from:"", // string
            to:"", // bitwise
            text:"" // string
       }

   ],
   timestamp: 0,
   signatura:"" //string
}

```

#get pool

## request

```javascript
/pool
```

## response

```javascript

{
   id:"", // packet id
   type:0, // bitwise
   timestamp: 0,
   signatura:"" //string
}

```





