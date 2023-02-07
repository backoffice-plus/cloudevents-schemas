# 



<table>
<tbody>
<tr><th>$id</th><td>io.miranum.bpmn.command.v1.CreateProcessInstanceRequest</td></tr>
<tr><th>$schema</th><td>http://json-schema.org/draft-07/schema#</td></tr>
</tbody>
</table>

## Properties

<table><thead><tr><th colspan="2">Name</th><th>Type</th></tr></thead><tbody><tr><td colspan="2"><a href="#processdefinitionkey">processDefinitionKey</a></td><td>Number</td></tr><tr><td colspan="2"><a href="#bpmnprocessid">bpmnProcessId</a></td><td>String</td></tr><tr><td colspan="2"><a href="#version">version</a></td><td>Number</td></tr><tr><td colspan="2"><a href="#variables">variables</a></td><td>String</td></tr><tr><td colspan="2"><a href="#startinstructions">startInstructions</a></td><td>Array</td></tr></tbody></table>



<hr />



## processDefinitionKey


<table>
  <tbody>
    <tr>
      <th>Description</th>
      <td colspan="2">the unique key identifying the process definition (e.g. returned from a process
in the DeployProcessResponse message)</td>
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
      <td colspan="2">the BPMN process ID of the process definition</td>
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
      <td colspan="2">the version of the process; set to -1 to use the latest version</td>
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
      <td colspan="2">JSON document that will instantiate the variables for the root variable scope of the
process instance; it must be a JSON object, as variables will be mapped in a
key-value fashion. e.g. { &quot;a&quot;: 1, &quot;b&quot;: 2 } will create two variables, named &quot;a&quot; and
&quot;b&quot; respectively, with their associated values. [{ &quot;a&quot;: 1, &quot;b&quot;: 2 }] would not be a
valid argument, as the root of the JSON document is an array and not an object.</td>
    </tr>
    <tr><th>Type</th><td colspan="2">String</td></tr>
    <tr>
      <th>Required</th>
      <td colspan="2">No</td>
    </tr>
    
  </tbody>
</table>






## startInstructions


<table>
  <tbody>
    <tr>
      <th>Description</th>
      <td colspan="2">List of start instructions. If empty (default) the process instance
will start at the start event. If non-empty the process instance will apply start
instructions after it has been created</td>
    </tr>
    <tr><th>Type</th><td colspan="2">Array</td></tr>
    <tr>
      <th>Required</th>
      <td colspan="2">No</td>
    </tr>
    
  </tbody>
</table>



### startInstructions.elementId


<table>
  <tbody>
    <tr>
      <th>Description</th>
      <td colspan="2">element ID</td>
    </tr>
    <tr><th>Type</th><td colspan="2">String</td></tr>
    
  </tbody>
</table>











<hr />

## Schema
```
{
    "$id": "io.miranum.bpmn.command.v1.CreateProcessInstanceRequest",
    "$schema": "http://json-schema.org/draft-07/schema#",
    "type": "object",
    "properties": {
        "processDefinitionKey": {
            "description": "the unique key identifying the process definition (e.g. returned from a process\nin the DeployProcessResponse message)",
            "type": "number"
        },
        "bpmnProcessId": {
            "description": "the BPMN process ID of the process definition",
            "type": "string"
        },
        "version": {
            "description": "the version of the process; set to -1 to use the latest version",
            "type": "number"
        },
        "variables": {
            "description": "JSON document that will instantiate the variables for the root variable scope of the\nprocess instance; it must be a JSON object, as variables will be mapped in a\nkey-value fashion. e.g. { \"a\": 1, \"b\": 2 } will create two variables, named \"a\" and\n\"b\" respectively, with their associated values. [{ \"a\": 1, \"b\": 2 }] would not be a\nvalid argument, as the root of the JSON document is an array and not an object.",
            "type": "string"
        },
        "startInstructions": {
            "description": "List of start instructions. If empty (default) the process instance\nwill start at the start event. If non-empty the process instance will apply start\ninstructions after it has been created",
            "type": "array",
            "items": {
                "$ref": "#/definitions/ProcessInstanceCreationStartInstruction"
            }
        }
    },
    "definitions": {
        "ProcessInstanceCreationStartInstruction": {
            "type": "object",
            "properties": {
                "elementId": {
                    "description": "element ID",
                    "type": "string"
                }
            }
        }
    }
}
```


