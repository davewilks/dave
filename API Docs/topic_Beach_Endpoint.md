#Resource description
*1-3 sentensce summary of the information the resource contains*
*Resources can be called: API calls
-Resources - a good generanl term
-Endpoints - use for the URL if describing them as resources. An API has various “resources” that you access through “endpoints.” The endpoint gives you access to a resource. The endpoint is the URL path (in this example, /surfreport). The information the endpoint interacts with, though, is called a resource.
-API methods
-Calls
-Resources
-Objects
-Services
-Requests*

*Describing a resource
-What does the resource contain? -- surfing conditions, height, water temp, wind and tide
-Beach ID
-Overall recommendation
-Broken down by hour*

**Returns information about surfing conditions at a specific beach ID, including the surf height, water temperature, wind, and tide. Also provides an overall recommendation about whether to go surfing.**

**{beachId} refers to the ID for the beach you want to look up. All Beach ID codes are available from our site.**
#Endpoint
*Endpoints can be called:
-Requests
-Endpoints
-API methods
-Resource URLs
-URLs
-URL syntax*

*When you describe the endpoint, it’s common to list the end path only (hence the nickname “endpoint”), e.g., just /surfreport/{beachId}.

*You don’t have to list the full URL every time (which would be https://simple-weather.p.mashape.com/surfreport{beachId}. Doing so distracts the user from focusing on the path that matters.*

*In your user guide, explain the full code path in an introductory section.*

*If you have path parameters in your endpoint, represent them through curly braces. For example, here’s an example from Mailchimp’s API:

/campaigns/**{campaign_id}**/actions/send

*Or use a completely different color, like red*

GET surfreport/{beachId}

#Methods
*Include with the endpoint*
#Parameters
*Parameters refer to the various ways the endpoint can be configured to influence the response. Many times parameters are out in a simple table like this:*

| Parameter | Required |Data Type | Example |
| --------- | -------- | --------- | ------- |
| Format | Optional | string | json |

*4 kinds of parameters*
*-Path parameters - in endpoint, before query string (?)
-Query string parameters, in endpoint after query string
-Request body - In body, usually JSON
-Header parameters - in header, usually related to authorization*

*Parameters should list allowed values*

*Consider color-coding parameters*
| Parameter | Required |Description | Type |
| --------- | -------- | --------- | ------- |
| days | Optional | The number of days to return surf information. The maximum is 7 and the default is 3. | integer |
| units | Optional | For feet choose imperial and for meters choose metric | string |
| days | Optional | The time of the day corresponding to time zone of the beach you're inquiring about | integer. Unix format (ms since 1970) in UTC |

#Request submission example
#Request response example
#Status and error codes
#Code samples
