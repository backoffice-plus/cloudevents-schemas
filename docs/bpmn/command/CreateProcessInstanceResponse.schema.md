# 



<table>
<tbody>
<tr><th>$id</th><td>io.miranum.bpmn.command.v1.CreateProcessInstanceResponse</td></tr>
<tr><th>$schema</th><td>http://json-schema.org/draft-07/schema#</td></tr>
</tbody>
</table>

## Properties

<table><thead><tr><th colspan="2">Name</th><th>Type</th></tr></thead><tbody><tr><td colspan="2"><a href="#processdefinitionkey">processDefinitionKey</a></td><td>Number</td></tr><tr><td colspan="2"><a href="#bpmnprocessid">bpmnProcessId</a></td><td>String</td></tr><tr><td colspan="2"><a href="#version">version</a></td><td>Number</td></tr><tr><td colspan="2"><a href="#processinstancekey">processInstanceKey</a></td><td>Number</td></tr></tbody></table>



<hr />



## processDefinitionKey


<table>
  <tbody>
    <tr>
      <th>Description</th>
      <td colspan="2">the key of the process definition which was used to create the process instance</td>
    </tr>
    <tr><th>Type</th><td colspan="2">Number</td></tr>
    <tr>
      <th>Required</th>
      <td colspan="2">No</td>
    </tr>
    
  </tbody>
</table>






## bpmnProcessId


<table>
  <tbody>
    <tr>
      <th>Description</th>
      <td colspan="2">the BPMN process ID of the process definition which was used to create the process
instance</td>
    </tr>
    <tr><th>Type</th><td colspan="2">String</td></tr>
    <tr>
      <th>Required</th>
      <td colspan="2">No</td>
    </tr>
    
  </tbody>
</table>






## version


<table>
  <tbody>
    <tr>
      <th>Description</th>
      <td colspan="2">the version of the process definition which was used to create the process instance</td>
    </tr>
    <tr><th>Type</th><td colspan="2">Number</td></tr>
    <tr>
      <th>Required</th>
      <td colspan="2">No</td>
    </tr>
    
  </tbody>
</table>






## processInstanceKey


<table>
  <tbody>
    <tr>
      <th>Description</th>
      <td colspan="2">the unique identifier of the created process instance; to be used wherever a request
needs a process instance key (e.g. CancelProcessInstanceRequest)</td>
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
    "$id": "io.miranum.bpmn.command.v1.CreateProcessInstanceResponse",
    "$schema": "http://json-schema.org/draft-07/schema#",
    "type": "object",
    "properties": {
        "processDefinitionKey": {
            "description": "the key of the process definition which was used to create the process instance",
            "type": "number"
        },
        "bpmnProcessId": {
            "description": "the BPMN process ID of the process definition which was used to create the process\ninstance",
            "type": "string"
        },
        "version": {
            "description": "the version of the process definition which was used to create the process instance",
            "type": "number"
        },
        "processInstanceKey": {
            "description": "the unique identifier of the created process instance; to be used wherever a request\nneeds a process instance key (e.g. CancelProcessInstanceRequest)",
            "type": "number"
        }
    }
}
```


