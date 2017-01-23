# Raw Arena

> Raw Arena

```json
{
  "Id": "cbis:1245084",
  "References": [
    "cbis:1245084"
  ],
  "Name": "Ewok",
  "GeoReferences": [],
  "Categories": [
    30701
  ],
  "InformationData": [
    {
      "Values": {
        "en-US": "Ewok"
      },
      "AttributeId": 99,
      "Type": "String"
    },
    {
      "Values": {
        "en-US": "Strongest animal ever, by far!"
      },
      "AttributeId": 101,
      "Type": "String"
    },
    {
      "Values": {
        "en-US": "Ewoks were a diminutive species of furry bipeds native to the forest moon of Endor. 
		They were most notable for helping the Rebel Alliance defeat the forces of the Galactic Empire 
		at the Battle of Endor, allowing the shield generator there to be destroyed, and in turn, the 
		Death Star II.\r\n\r\nEwoks were individuals that stood about one meter tall; they used spears, 
		slings, and knives as weapons; they also used hang gliders as vehicles. Although skilled in forest 
		survival and the construction of primitive technology, the Ewoks had yet to progress past 
		stone-level technology when discovered by the Empire. They were quick learners, however, when 
		exposed to advanced technology with simple mechanical processes and concepts."
      },
      "AttributeId": 102,
      "Type": "String"
    }
  ],
  "Position": {
      "Longitude": 7.1934700012207,
      "Latitude": 48.172353561064
    },
  "ExpiresAt": "2018-07-01T01:00:00",
  "PublishAt": null,
  "Occasions": [
    {
      "Start": "2016-06-16T00:00:00",
      "End": "2016-06-30T00:00:00",
      "StartTime": 0,
      "Duration": 864000000000,
      "Days": 127,
      "IsRecurring": true,
      "Monday": true,
      "Tuesday": true,
      "Wednesday": true,
      "Thursday": true,
      "Friday": true,
      "Saturday": true,
      "Sunday": true,
      "ArenaId": ""
    }
  ],
  "Media": [
    {
      "Url": "http://images.citybreak.com/image.aspx?ImageId=4161317",
      "Type": "MainImage",
      "Name": {},
      "Description": {},
      "Copyright": null
    },
    {
      "Url": "http://images.citybreak.com/image.aspx?ImageId=4223191",
      "Type": "Image",
      "Name": {},
      "Description": {},
      "Copyright": null
    }
  ],
  "Pois": [],
  "Type": "Arena"
}
```

All the info we have about your arenas.

## Get Arena

```shell
curl -X GET 
  --header 'ApiKey: APIKEY132456789EWOK'
  --header 'Accept: application/json' 
  'https://cbis-rest-api.citybreak.com/v1/api/raw/arena/{id}'
```

```javascript
var r = fetch("https://cbis-rest-api.citybreak.com/v1/api/raw/arena/{id}",
{
  headers: {
    "ApiKey:" "APIKEY132456789EWOK",
    "Accept": "application/json"
  }  
});
```

> Example of response:

```json
[
  {
    "Id": "cbis:1245084",
    "References": [
      "cbis:1245084"
    ],
    "Name": "Ewok",
    "GeoReferences": [],
    "Categories": [
      30701
    ],
    "InformationData": [
      {
        "Values": {
          "en-US": "Ewok"
        },
        "AttributeId": 99,
        "Type": "String"
      },
      {
        "Values": {
          "en-US": "Strongest animal ever, by far!"
        },
        "AttributeId": 101,
        "Type": "String"
      },
      {
        "Values": {
          "en-US": "Ewoks were a diminutive species of furry bipeds native to the forest moon of Endor. 
		  They were most notable for helping the Rebel Alliance defeat the forces of the Galactic Empire 
		  at the Battle of Endor, allowing the shield generator there to be destroyed, and in turn, the 
		  Death Star II.\r\n\r\nEwoks were individuals that stood about one meter tall; they used spears, 
		  slings, and knives as weapons; they also used hang gliders as vehicles. Although skilled in forest 
		  survival and the construction of primitive technology, the Ewoks had yet to progress past 
		  stone-level technology when discovered by the Empire. They were quick learners, however, when 
		  exposed to advanced technology with simple mechanical processes and concepts."
        },
        "AttributeId": 102,
        "Type": "String"
      }
    ],
    "Position": {
      "Longitude": 7.1934700012207,
      "Latitude": 48.172353561064
    },
    "ExpiresAt": "2018-07-01T01:00:00",
    "PublishAt": null,
    "Occasions": [
      {
        "Start": "2016-06-16T00:00:00",
        "End": "2016-06-30T00:00:00",
        "StartTime": 0,
        "Duration": 864000000000,
        "Days": 127,
        "IsRecurring": true,
        "Monday": true,
        "Tuesday": true,
        "Wednesday": true,
        "Thursday": true,
        "Friday": true,
        "Saturday": true,
        "Sunday": true,
        "ArenaId": ""
      }
    ],
    "Medias": [
      {
        "Url": "http://images.citybreak.com/image.aspx?ImageId=4161317",
        "Type": "MainImage",
        "Name": {},
        "Description": {},
        "Copyright": null
      },
      {
        "Url": "http://images.citybreak.com/image.aspx?ImageId=4223191",
        "Type": "Image",
        "Name": {},
        "Description": {},
        "Copyright": null
      }
    ],
    "Pois": [],
    "Type": "Arena"
  }
]
```

Search for arenas answering to the id provided, might be more than 1.

### HTTP Request

`GET https://cbis-rest-api.citybreak.com/v1/api/raw/arena/{id}`

### Query Parameters

Parameter | Description
--------- | -----------
id | The arena id.

## Get Paged

```shell
curl -X GET 
  --header 'ApiKey: APIKEY132456789EWOK'
  --header 'Accept: application/json' 
  'https://cbis-rest-api.citybreak.com/v1/api/raw/arena/getpaged/{pageSize}'
```

```javascript
var r = fetch("https://cbis-rest-api.citybreak.com/v1/api/raw/Arena/getpaged/{pageSize}",
{
  headers: {
    "ApiKey:" "APIKEY132456789EWOK",
    "Accept": "application/json"
  }  
});
```

> Example of response:

```json
{
  "ContinueToken": "c2NhbjswOzE7dG90YWxfaGl0czo0Ow==",
  "TotalResults": 4,
  "Result": [
    {
    "Id": "cbis:1245084",
    "References": [
      "cbis:1245084"
    ],
    "Name": "Ewok",
    "GeoReferences": [],
    "Categories": [
      30701
    ],
    "InformationData": [
      {
        "Values": {
          "en-US": "Ewok"
        },
        "AttributeId": 99,
        "Type": "String"
      },
      {
        "Values": {
          "en-US": "Strongest animal ever, by far!"
        },
        "AttributeId": 101,
        "Type": "String"
      },
      {
        "Values": {
          "en-US": "Ewoks were a diminutive species of furry bipeds native to the forest moon of Endor. 
		  They were most notable for helping the Rebel Alliance defeat the forces of the Galactic Empire 
		  at the Battle of Endor, allowing the shield generator there to be destroyed, and in turn, the 
		  Death Star II.\r\n\r\nEwoks were individuals that stood about one meter tall; they used spears, 
		  slings, and knives as weapons; they also used hang gliders as vehicles. Although skilled in forest 
		  survival and the construction of primitive technology, the Ewoks had yet to progress past 
		  stone-level technology when discovered by the Empire. They were quick learners, however, when 
		  exposed to advanced technology with simple mechanical processes and concepts."
        },
        "AttributeId": 102,
        "Type": "String"
      }
    ],
    "Position": {
      "Longitude": 7.1934700012207,
      "Latitude": 48.172353561064
    },
    "ExpiresAt": "2018-07-01T01:00:00",
    "PublishAt": null,
    "Occasions": [
      {
        "Start": "2016-06-16T00:00:00",
        "End": "2016-06-30T00:00:00",
        "StartTime": 0,
        "Duration": 864000000000,
        "Days": 127,
        "IsRecurring": true,
        "Monday": true,
        "Tuesday": true,
        "Wednesday": true,
        "Thursday": true,
        "Friday": true,
        "Saturday": true,
        "Sunday": true,
        "ArenaId": ""
      }
    ],
    "Medias": [
      {
        "Url": "http://images.citybreak.com/image.aspx?ImageId=4161317",
        "Type": "MainImage",
        "Name": {},
        "Description": {},
        "Copyright": null
      },
      {
        "Url": "http://images.citybreak.com/image.aspx?ImageId=4223191",
        "Type": "Image",
        "Name": {},
        "Description": {},
        "Copyright": null
      }
    ],
    "Pois": [],
    "Type": "Arena"
  }
  ]
}
```

Get a page of raw arenas.

### HTTP Request

`GET https://cbis-rest-api.citybreak.com/v1/api/raw/arena/getpaged/{pageSize}`

### Query Parameters

Parameter | Description
--------- | -----------
pageSize | Should be a page size lower than 50 and greater than 0.


<aside class="notice">
Use the <a href="https://visit.github.io/api-doc/#continue29">ContinueToken</a> to grab the next page until you get an <b>empty</b> result set.
</aside>

## Continue

```shell
curl -X GET 
  --header 'ApiKey: APIKEY132456789EWOK'
  --header 'Accept: application/json' 
  'https://cbis-rest-api.citybreak.com/v1/api/raw/arena/getnext/{continueToken}'
```

```javascript
var r = fetch("https://cbis-rest-api.citybreak.com/v1/api/raw/arena/getnext/{continueToken}",
{
  headers: {
    "ApiKey:" "APIKEY132456789EWOK",
    "Accept": "application/json"
  }  
});
```

> Example of response:

```json
{
  "ContinueToken": "c2NhbjswOzE7dG90YWxfaGl0czo0Ow==",
  "TotalResults": 4,
  "Result": [
    {
    "Id": "cbis:1245084",
    "References": [
      "cbis:1245084"
    ],
    "Name": "Ewok",
    "GeoReferences": [],
    "Categories": [
      30701
    ],
    "InformationData": [
      {
        "Values": {
          "en-US": "Ewok"
        },
        "AttributeId": 99,
        "Type": "String"
      },
      {
        "Values": {
          "en-US": "Strongest animal ever, by far!"
        },
        "AttributeId": 101,
        "Type": "String"
      },
      {
        "Values": {
          "en-US": "Ewoks were a diminutive species of furry bipeds native to the forest moon of Endor. 
		  They were most notable for helping the Rebel Alliance defeat the forces of the Galactic Empire 
		  at the Battle of Endor, allowing the shield generator there to be destroyed, and in turn, the 
		  Death Star II.\r\n\r\nEwoks were individuals that stood about one meter tall; they used spears, 
		  slings, and knives as weapons; they also used hang gliders as vehicles. Although skilled in forest 
		  survival and the construction of primitive technology, the Ewoks had yet to progress past 
		  stone-level technology when discovered by the Empire. They were quick learners, however, when 
		  exposed to advanced technology with simple mechanical processes and concepts."
        },
        "AttributeId": 102,
        "Type": "String"
      }
    ],
    "Position": {
      "Longitude": 7.1934700012207,
      "Latitude": 48.172353561064
    },
    "ExpiresAt": "2018-07-01T01:00:00",
    "PublishAt": null,
    "Occasions": [
      {
        "Start": "2016-06-16T00:00:00",
        "End": "2016-06-30T00:00:00",
        "StartTime": 0,
        "Duration": 864000000000,
        "Days": 127,
        "IsRecurring": true,
        "Monday": true,
        "Tuesday": true,
        "Wednesday": true,
        "Thursday": true,
        "Friday": true,
        "Saturday": true,
        "Sunday": true,
        "ArenaId": ""
      }
    ],
    "Medias": [
      {
        "Url": "http://images.citybreak.com/image.aspx?ImageId=4161317",
        "Type": "MainImage",
        "Name": {},
        "Description": {},
        "Copyright": null
      },
      {
        "Url": "http://images.citybreak.com/image.aspx?ImageId=4223191",
        "Type": "Image",
        "Name": {},
        "Description": {},
        "Copyright": null
      }
    ],
    "Pois": [],
    "Type": "Arena"
  }
  ]
}
```

Get the next page of raw arenas, you need to provide a token obtained from <a href="https://visit.github.io/api-doc/#get-paged28">Get Paged</a>.

### HTTP Request

`GET https://cbis-rest-api.citybreak.com/v1/api/raw/arena/getnext/{continueToken}`

### Query Parameters

Parameter | Description
--------- | -----------
continueToken | A token to retrieve the next page.


<aside class="notice">
Use the <a href="https://visit.github.io/api-doc/#continue29">ContinueToken</a> to grab the next page until you get an <b>empty</b> result set.
</aside>