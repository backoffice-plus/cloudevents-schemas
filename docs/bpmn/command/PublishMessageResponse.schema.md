# 



<table>
<tbody>
<tr><th>$id</th><td>io.miranum.bpmn.command.v1.PublishMessageResponse</td></tr>
<tr><th>$schema</th><td>http://json-schema.org/draft-07/schema#</td></tr>
</tbody>
</table>

## Properties

<table><thead><tr><th colspan="2">Name</th><th>Type</th></tr></thead><tbody><tr><td colspan="2"><a href="#key">key</a></td><td>Number</td></tr></tbody></table>



<hr />



## key


<table>
  <tbody>
    <tr>
      <th>Description</th>
      <td colspan="2">the unique ID of the message that was published</td>
    </tr>
    <tr><th>Type</th><td colspan="2">Number</td></tr>
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
    "$id": "io.miranum.bpmn.command.v1.PublishMessageResponse",
    "$schema": "http://json-schema.org/draft-07/schema#",
    "type": "object",
    "properties": {
        "key": {
            "description": "the unique ID of the message that was published",
            "type": "number"
        }
    }
}
```


