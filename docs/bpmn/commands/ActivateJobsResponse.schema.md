# 



<table>
<tbody>
<tr><th>$id</th><td>io.miranum.bpmn.command.v1.ActivateJobsResponse</td></tr>
<tr><th>$schema</th><td>http://json-schema.org/draft-07/schema#</td></tr>
</tbody>
</table>

## Properties

<table><thead><tr><th colspan="2">Name</th><th>Type</th></tr></thead><tbody><tr><td colspan="2"><a href="#jobs">jobs</a></td><td>Array</td></tr></tbody></table>



<hr />



## jobs


<table>
  <tbody>
    <tr>
      <th>Description</th>
      <td colspan="2">list of activated jobs</td>
    </tr>
    <tr><th>Type</th><td colspan="2">Array</td></tr>
    <tr>
      <th>Required</th>
      <td colspan="2">No</td>
    </tr>
    
  </tbody>
</table>



### jobs.key


<table>
  <tbody>
    <tr>
      <th>Description</th>
      <td colspan="2">the key, a unique identifier for the job</td>
    </tr>
    <tr><th>Type</th><td colspan="2">Number</td></tr>
    
  </tbody>
</table>




### jobs.type


<table>
  <tbody>
    <tr>
      <th>Description</th>
      <td colspan="2">the type of the job (should match what was requested)</td>
    </tr>
    <tr><th>Type</th><td colspan="2">String</td></tr>
    
  </tbody>
</table>




### jobs.processInstanceKey


<table>
  <tbody>
    <tr>
      <th>Description</th>
      <td colspan="2">the job&#x27;s process instance key</td>
    </tr>
    <tr><th>Type</th><td colspan="2">Number</td></tr>
    
  </tbody>
</table>




### jobs.bpmnProcessId


<table>
  <tbody>
    <tr>
      <th>Description</th>
      <td colspan="2">the bpmn process ID of the job process definition</td>
    </tr>
    <tr><th>Type</th><td colspan="2">String</td></tr>
    
  </tbody>
</table>




### jobs.processDefinitionVersion


<table>
  <tbody>
    <tr>
      <th>Description</th>
      <td colspan="2">the version of the job process definition</td>
    </tr>
    <tr><th>Type</th><td colspan="2">Number</td></tr>
    
  </tbody>
</table>




### jobs.processDefinitionKey


<table>
  <tbody>
    <tr>
      <th>Description</th>
      <td colspan="2">the key of the job process definition</td>
    </tr>
    <tr><th>Type</th><td colspan="2">Number</td></tr>
    
  </tbody>
</table>




### jobs.elementId


<table>
  <tbody>
    <tr>
      <th>Description</th>
      <td colspan="2">the associated task element ID</td>
    </tr>
    <tr><th>Type</th><td colspan="2">String</td></tr>
    
  </tbody>
</table>




### jobs.elementInstanceKey


<table>
  <tbody>
    <tr>
      <th>Description</th>
      <td colspan="2">the unique key identifying the associated task, unique within the scope of the
process instance</td>
    </tr>
    <tr><th>Type</th><td colspan="2">Number</td></tr>
    
  </tbody>
</table>




### jobs.customHeaders


<table>
  <tbody>
    <tr>
      <th>Description</th>
      <td colspan="2">a set of custom headers defined during modelling; returned as a serialized
JSON document</td>
    </tr>
    <tr><th>Type</th><td colspan="2">String</td></tr>
    
  </tbody>
</table>




### jobs.worker


<table>
  <tbody>
    <tr>
      <th>Description</th>
      <td colspan="2">the name of the worker which activated this job</td>
    </tr>
    <tr><th>Type</th><td colspan="2">String</td></tr>
    
  </tbody>
</table>




### jobs.retries


<table>
  <tbody>
    <tr>
      <th>Description</th>
      <td colspan="2">the amount of retries left to this job (should always be positive)</td>
    </tr>
    <tr><th>Type</th><td colspan="2">Number</td></tr>
    
  </tbody>
</table>




### jobs.deadline


<table>
  <tbody>
    <tr>
      <th>Description</th>
      <td colspan="2">when the job can be activated again, sent as a UNIX epoch timestamp</td>
    </tr>
    <tr><th>Type</th><td colspan="2">Number</td></tr>
    
  </tbody>
</table>




### jobs.variables


<table>
  <tbody>
    <tr>
      <th>Description</th>
      <td colspan="2">JSON document, computed at activation time, consisting of all visible variables to
the task scope</td>
    </tr>
    <tr><th>Type</th><td colspan="2">String</td></tr>
    
  </tbody>
</table>











<hr />

## Schema
```
{
    "$id": "io.miranum.bpmn.command.v1.ActivateJobsResponse",
    "$schema": "http://json-schema.org/draft-07/schema#",
    "type": "object",
    "properties": {
        "jobs": {
            "description": "list of activated jobs",
            "type": "array",
            "items": {
                "$ref": "#/definitions/ActivatedJob"
            }
        }
    },
    "definitions": {
        "ActivatedJob": {
            "type": "object",
            "properties": {
                "key": {
                    "description": "the key, a unique identifier for the job",
                    "type": "number"
                },
                "type": {
                    "description": "the type of the job (should match what was requested)",
                    "type": "string"
                },
                "processInstanceKey": {
                    "description": "the job's process instance key",
                    "type": "number"
                },
                "bpmnProcessId": {
                    "description": "the bpmn process ID of the job process definition",
                    "type": "string"
                },
                "processDefinitionVersion": {
                    "description": "the version of the job process definition",
                    "type": "number"
                },
                "processDefinitionKey": {
                    "description": "the key of the job process definition",
                    "type": "number"
                },
                "elementId": {
                    "description": "the associated task element ID",
                    "type": "string"
                },
                "elementInstanceKey": {
                    "description": "the unique key identifying the associated task, unique within the scope of the\nprocess instance",
                    "type": "number"
                },
                "customHeaders": {
                    "description": "a set of custom headers defined during modelling; returned as a serialized\nJSON document",
                    "type": "string"
                },
                "worker": {
                    "description": "the name of the worker which activated this job",
                    "type": "string"
                },
                "retries": {
                    "description": "the amount of retries left to this job (should always be positive)",
                    "type": "number"
                },
                "deadline": {
                    "description": "when the job can be activated again, sent as a UNIX epoch timestamp",
                    "type": "number"
                },
                "variables": {
                    "description": "JSON document, computed at activation time, consisting of all visible variables to\nthe task scope",
                    "type": "string"
                }
            }
        }
    }
}
```


