# 



<table>
<tbody>
<tr><th>$id</th><td>io.miranum.bpmn.command.v1.CancelProcessInstanceRequest</td></tr>
<tr><th>$schema</th><td>http://json-schema.org/draft-07/schema#</td></tr>
</tbody>
</table>

## Properties

<table><thead><tr><th colspan="2">Name</th><th>Type</th></tr></thead><tbody><tr><td colspan="2"><a href="#processinstancekey">processInstanceKey</a></td><td>Number</td></tr></tbody></table>



<hr />



## processInstanceKey


<table>
  <tbody>
    <tr>
      <th>Description</th>
      <td colspan="2">the process instance key (as, for example, obtained from
CreateProcessInstanceResponse)</td>
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
    "$id": "io.miranum.bpmn.command.v1.CancelProcessInstanceRequest",
    "$schema": "http://json-schema.org/draft-07/schema#",
    "type": "object",
    "properties": {
        "processInstanceKey": {
            "description": "the process instance key (as, for example, obtained from\nCreateProcessInstanceResponse)",
            "type": "number"
        }
    }
}
```


