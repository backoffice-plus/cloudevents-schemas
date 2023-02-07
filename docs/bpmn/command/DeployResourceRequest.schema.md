# 



<table>
<tbody>
<tr><th>$id</th><td>io.miranum.bpmn.command.v1.DeployResourceRequest</td></tr>
<tr><th>$schema</th><td>http://json-schema.org/draft-07/schema#</td></tr>
</tbody>
</table>

## Properties

<table><thead><tr><th colspan="2">Name</th><th>Type</th></tr></thead><tbody><tr><td colspan="2"><a href="#resources">resources</a></td><td>Array</td></tr></tbody></table>



<hr />



## resources


<table>
  <tbody>
    <tr>
      <th>Description</th>
      <td colspan="2">list of resources to deploy</td>
    </tr>
    <tr><th>Type</th><td colspan="2">Array</td></tr>
    <tr>
      <th>Required</th>
      <td colspan="2">No</td>
    </tr>
    
  </tbody>
</table>



### resources.name


<table>
  <tbody>
    <tr>
      <th>Description</th>
      <td colspan="2">the resource name, e.g. myProcess.bpmn or myDecision.dmn</td>
    </tr>
    <tr><th>Type</th><td colspan="2">String</td></tr>
    
  </tbody>
</table>




### resources.content


<table>
  <tbody>
    <tr>
      <th>Description</th>
      <td colspan="2">the file content as a UTF8-encoded string
The content must be base64 encoded.</td>
    </tr>
    <tr><th>Type</th><td colspan="2">String</td></tr>
    
  </tbody>
</table>











<hr />

## Schema
```
{
    "$id": "io.miranum.bpmn.command.v1.DeployResourceRequest",
    "$schema": "http://json-schema.org/draft-07/schema#",
    "type": "object",
    "properties": {
        "resources": {
            "description": "list of resources to deploy",
            "type": "array",
            "items": {
                "$ref": "#/definitions/Resource"
            }
        }
    },
    "definitions": {
        "Resource": {
            "type": "object",
            "properties": {
                "name": {
                    "description": "the resource name, e.g. myProcess.bpmn or myDecision.dmn",
                    "type": "string"
                },
                "content": {
                    "description": "the file content as a UTF8-encoded string\nThe content must be base64 encoded.",
                    "type": "string"
                }
            }
        }
    }
}
```


