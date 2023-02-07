# 



<table>
<tbody>
<tr><th>$id</th><td>io.miranum.bpmn.command.v1.CompleteJobRequest</td></tr>
<tr><th>$schema</th><td>http://json-schema.org/draft-07/schema#</td></tr>
</tbody>
</table>

## Properties

<table><thead><tr><th colspan="2">Name</th><th>Type</th></tr></thead><tbody><tr><td colspan="2"><a href="#jobkey">jobKey</a></td><td>Number</td></tr><tr><td colspan="2"><a href="#variables">variables</a></td><td>String</td></tr></tbody></table>



<hr />



## jobKey


<table>
  <tbody>
    <tr>
      <th>Description</th>
      <td colspan="2">the unique job identifier, as obtained from ActivateJobsResponse</td>
    </tr>
    <tr><th>Type</th><td colspan="2">Number</td></tr>
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
      <td colspan="2">a JSON document representing the variables in the current task scope</td>
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
    "$id": "io.miranum.bpmn.command.v1.CompleteJobRequest",
    "$schema": "http://json-schema.org/draft-07/schema#",
    "type": "object",
    "properties": {
        "jobKey": {
            "description": "the unique job identifier, as obtained from ActivateJobsResponse",
            "type": "number"
        },
        "variables": {
            "description": "a JSON document representing the variables in the current task scope",
            "type": "string"
        }
    }
}
```


