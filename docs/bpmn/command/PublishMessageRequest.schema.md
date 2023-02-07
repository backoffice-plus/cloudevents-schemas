# 



<table>
<tbody>
<tr><th>$id</th><td>io.miranum.bpmn.command.v1.PublishMessageRequest</td></tr>
<tr><th>$schema</th><td>http://json-schema.org/draft-07/schema#</td></tr>
</tbody>
</table>

## Properties

<table><thead><tr><th colspan="2">Name</th><th>Type</th></tr></thead><tbody><tr><td colspan="2"><a href="#name">name</a></td><td>String</td></tr><tr><td colspan="2"><a href="#correlationkey">correlationKey</a></td><td>String</td></tr><tr><td colspan="2"><a href="#timetolive">timeToLive</a></td><td>Number</td></tr><tr><td colspan="2"><a href="#messageid">messageId</a></td><td>String</td></tr><tr><td colspan="2"><a href="#variables">variables</a></td><td>String</td></tr></tbody></table>



<hr />



## name


<table>
  <tbody>
    <tr>
      <th>Description</th>
      <td colspan="2">the name of the message</td>
    </tr>
    <tr><th>Type</th><td colspan="2">String</td></tr>
    <tr>
      <th>Required</th>
      <td colspan="2">No</td>
    </tr>
    
  </tbody>
</table>






## correlationKey


<table>
  <tbody>
    <tr>
      <th>Description</th>
      <td colspan="2">the correlation key of the message</td>
    </tr>
    <tr><th>Type</th><td colspan="2">String</td></tr>
    <tr>
      <th>Required</th>
      <td colspan="2">No</td>
    </tr>
    
  </tbody>
</table>






## timeToLive


<table>
  <tbody>
    <tr>
      <th>Description</th>
      <td colspan="2">how long the message should be buffered on the broker, in milliseconds</td>
    </tr>
    <tr><th>Type</th><td colspan="2">Number</td></tr>
    <tr>
      <th>Required</th>
      <td colspan="2">No</td>
    </tr>
    
  </tbody>
</table>






## messageId


<table>
  <tbody>
    <tr>
      <th>Description</th>
      <td colspan="2">the unique ID of the message; can be omitted. only useful to ensure only one message
with the given ID will ever be published (during its lifetime)</td>
    </tr>
    <tr><th>Type</th><td colspan="2">String</td></tr>
    <tr>
      <th>Required</th>
      <td colspan="2">No</td>
    </tr>
    
  </tbody>
</table>






## variables


<table>
  <tbody>
    <tr>
      <th>Description</th>
      <td colspan="2">the message variables as a JSON document; to be valid, the root of the document must be an
object, e.g. { &quot;a&quot;: &quot;foo&quot; }. [ &quot;foo&quot; ] would not be valid.</td>
    </tr>
    <tr><th>Type</th><td colspan="2">String</td></tr>
    <tr>
      <th>Required</th>
      <td colspan="2">No</td>
    </tr>
    
  </tbody>
</table>










<hr />

## Schema
```
{
    "$id": "io.miranum.bpmn.command.v1.PublishMessageRequest",
    "$schema": "http://json-schema.org/draft-07/schema#",
    "type": "object",
    "properties": {
        "name": {
            "description": "the name of the message",
            "type": "string"
        },
        "correlationKey": {
            "description": "the correlation key of the message",
            "type": "string"
        },
        "timeToLive": {
            "description": "how long the message should be buffered on the broker, in milliseconds",
            "type": "number"
        },
        "messageId": {
            "description": "the unique ID of the message; can be omitted. only useful to ensure only one message\nwith the given ID will ever be published (during its lifetime)",
            "type": "string"
        },
        "variables": {
            "description": "the message variables as a JSON document; to be valid, the root of the document must be an\nobject, e.g. { \"a\": \"foo\" }. [ \"foo\" ] would not be valid.",
            "type": "string"
        }
    }
}
```


