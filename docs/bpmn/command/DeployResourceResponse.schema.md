# 



<table>
<tbody>
<tr><th>$id</th><td>io.miranum.bpmn.command.v1.DeployResourceResponse</td></tr>
<tr><th>$schema</th><td>http://json-schema.org/draft-07/schema#</td></tr>
</tbody>
</table>

## Properties

<table><thead><tr><th colspan="2">Name</th><th>Type</th></tr></thead><tbody><tr><td colspan="2"><a href="#key">key</a></td><td>Number</td></tr><tr><td colspan="2"><a href="#deployments">deployments</a></td><td>Array</td></tr></tbody></table>



<hr />



## key


<table>
  <tbody>
    <tr>
      <th>Description</th>
      <td colspan="2">the unique key identifying the deployment</td>
    </tr>
    <tr><th>Type</th><td colspan="2">Number</td></tr>
    <tr>
      <th>Required</th>
      <td colspan="2">No</td>
    </tr>
    
  </tbody>
</table>






## deployments


<table>
  <tbody>
    <tr>
      <th>Description</th>
      <td colspan="2">a list of deployed resources, e.g. processes</td>
    </tr>
    <tr><th>Type</th><td colspan="2">Array</td></tr>
    <tr>
      <th>Required</th>
      <td colspan="2">No</td>
    </tr>
    
  </tbody>
</table>



### deployments.process


<table>
  <tbody>
    <tr>
      <th>Description</th>
      <td colspan="2">metadata of a deployed process</td>
    </tr>
    <tr><th>Type</th><td colspan="2">Object</td></tr>
    
  </tbody>
</table>



### deployments.process.bpmnProcessId


<table>
  <tbody>
    <tr>
      <th>Description</th>
      <td colspan="2">the bpmn process ID, as parsed during deployment; together with the version forms a
unique identifier for a specific process definition</td>
    </tr>
    <tr><th>Type</th><td colspan="2">String</td></tr>
    
  </tbody>
</table>




### deployments.process.version


<table>
  <tbody>
    <tr>
      <th>Description</th>
      <td colspan="2">the assigned process version</td>
    </tr>
    <tr><th>Type</th><td colspan="2">Number</td></tr>
    
  </tbody>
</table>




### deployments.process.processDefinitionKey


<table>
  <tbody>
    <tr>
      <th>Description</th>
      <td colspan="2">the assigned key, which acts as a unique identifier for this process</td>
    </tr>
    <tr><th>Type</th><td colspan="2">Number</td></tr>
    
  </tbody>
</table>




### deployments.process.resourceName


<table>
  <tbody>
    <tr>
      <th>Description</th>
      <td colspan="2">the resource name (see: ProcessRequestObject.name) from which this process was
parsed</td>
    </tr>
    <tr><th>Type</th><td colspan="2">String</td></tr>
    
  </tbody>
</table>





### deployments.decision


<table>
  <tbody>
    <tr>
      <th>Description</th>
      <td colspan="2">metadata of a deployed decision</td>
    </tr>
    <tr><th>Type</th><td colspan="2">Object</td></tr>
    
  </tbody>
</table>



### deployments.decision.dmnDecisionId


<table>
  <tbody>
    <tr>
      <th>Description</th>
      <td colspan="2">the dmn decision ID, as parsed during deployment; together with the
versions forms a unique identifier for a specific decision</td>
    </tr>
    <tr><th>Type</th><td colspan="2">String</td></tr>
    
  </tbody>
</table>




### deployments.decision.dmnDecisionName


<table>
  <tbody>
    <tr>
      <th>Description</th>
      <td colspan="2">the dmn name of the decision, as parsed during deployment</td>
    </tr>
    <tr><th>Type</th><td colspan="2">String</td></tr>
    
  </tbody>
</table>




### deployments.decision.version


<table>
  <tbody>
    <tr>
      <th>Description</th>
      <td colspan="2">the assigned decision version</td>
    </tr>
    <tr><th>Type</th><td colspan="2">Number</td></tr>
    
  </tbody>
</table>




### deployments.decision.decisionKey


<table>
  <tbody>
    <tr>
      <th>Description</th>
      <td colspan="2">the assigned decision key, which acts as a unique identifier for this
decision</td>
    </tr>
    <tr><th>Type</th><td colspan="2">Number</td></tr>
    
  </tbody>
</table>




### deployments.decision.dmnDecisionRequirementsId


<table>
  <tbody>
    <tr>
      <th>Description</th>
      <td colspan="2">the dmn ID of the decision requirements graph that this decision is part
of, as parsed during deployment</td>
    </tr>
    <tr><th>Type</th><td colspan="2">String</td></tr>
    
  </tbody>
</table>




### deployments.decision.decisionRequirementsKey


<table>
  <tbody>
    <tr>
      <th>Description</th>
      <td colspan="2">the assigned key of the decision requirements graph that this decision is
part of</td>
    </tr>
    <tr><th>Type</th><td colspan="2">Number</td></tr>
    
  </tbody>
</table>





### deployments.decisionRequirements


<table>
  <tbody>
    <tr>
      <th>Description</th>
      <td colspan="2">metadata of a deployed decision requirements</td>
    </tr>
    <tr><th>Type</th><td colspan="2">Object</td></tr>
    
  </tbody>
</table>



### deployments.decisionRequirements.dmnDecisionRequirementsId


<table>
  <tbody>
    <tr>
      <th>Description</th>
      <td colspan="2">the dmn decision requirements ID, as parsed during deployment; together
with the versions forms a unique identifier for a specific decision</td>
    </tr>
    <tr><th>Type</th><td colspan="2">String</td></tr>
    
  </tbody>
</table>




### deployments.decisionRequirements.dmnDecisionRequirementsName


<table>
  <tbody>
    <tr>
      <th>Description</th>
      <td colspan="2">the dmn name of the decision requirements, as parsed during deployment</td>
    </tr>
    <tr><th>Type</th><td colspan="2">String</td></tr>
    
  </tbody>
</table>




### deployments.decisionRequirements.version


<table>
  <tbody>
    <tr>
      <th>Description</th>
      <td colspan="2">the assigned decision requirements version</td>
    </tr>
    <tr><th>Type</th><td colspan="2">Number</td></tr>
    
  </tbody>
</table>




### deployments.decisionRequirements.decisionRequirementsKey


<table>
  <tbody>
    <tr>
      <th>Description</th>
      <td colspan="2">the assigned decision requirements key, which acts as a unique identifier
for this decision requirements</td>
    </tr>
    <tr><th>Type</th><td colspan="2">Number</td></tr>
    
  </tbody>
</table>




### deployments.decisionRequirements.resourceName


<table>
  <tbody>
    <tr>
      <th>Description</th>
      <td colspan="2">the resource name (see: Resource.name) from which this decision
requirements was parsed</td>
    </tr>
    <tr><th>Type</th><td colspan="2">String</td></tr>
    
  </tbody>
</table>












<hr />

## Schema
```
{
    "$id": "io.miranum.bpmn.command.v1.DeployResourceResponse",
    "$schema": "http://json-schema.org/draft-07/schema#",
    "type": "object",
    "properties": {
        "key": {
            "description": "the unique key identifying the deployment",
            "type": "number"
        },
        "deployments": {
            "description": "a list of deployed resources, e.g. processes",
            "type": "array",
            "items": {
                "$ref": "#/definitions/Deployment"
            }
        }
    },
    "definitions": {
        "Deployment": {
            "type": "object",
            "properties": {
                "process": {
                    "description": "metadata of a deployed process",
                    "$ref": "#/definitions/ProcessMetadata"
                },
                "decision": {
                    "description": "metadata of a deployed decision",
                    "$ref": "#/definitions/DecisionMetadata"
                },
                "decisionRequirements": {
                    "description": "metadata of a deployed decision requirements",
                    "$ref": "#/definitions/DecisionRequirementsMetadata"
                }
            }
        },
        "ProcessMetadata": {
            "type": "object",
            "properties": {
                "bpmnProcessId": {
                    "description": "the bpmn process ID, as parsed during deployment; together with the version forms a\nunique identifier for a specific process definition",
                    "type": "string"
                },
                "version": {
                    "description": "the assigned process version",
                    "type": "number"
                },
                "processDefinitionKey": {
                    "description": "the assigned key, which acts as a unique identifier for this process",
                    "type": "number"
                },
                "resourceName": {
                    "description": "the resource name (see: ProcessRequestObject.name) from which this process was\nparsed",
                    "type": "string"
                }
            }
        },
        "DecisionMetadata": {
            "type": "object",
            "properties": {
                "dmnDecisionId": {
                    "description": "the dmn decision ID, as parsed during deployment; together with the\nversions forms a unique identifier for a specific decision",
                    "type": "string"
                },
                "dmnDecisionName": {
                    "description": "the dmn name of the decision, as parsed during deployment",
                    "type": "string"
                },
                "version": {
                    "description": "the assigned decision version",
                    "type": "number"
                },
                "decisionKey": {
                    "description": "the assigned decision key, which acts as a unique identifier for this\ndecision",
                    "type": "number"
                },
                "dmnDecisionRequirementsId": {
                    "description": "the dmn ID of the decision requirements graph that this decision is part\nof, as parsed during deployment",
                    "type": "string"
                },
                "decisionRequirementsKey": {
                    "description": "the assigned key of the decision requirements graph that this decision is\npart of",
                    "type": "number"
                }
            }
        },
        "DecisionRequirementsMetadata": {
            "type": "object",
            "properties": {
                "dmnDecisionRequirementsId": {
                    "description": "the dmn decision requirements ID, as parsed during deployment; together\nwith the versions forms a unique identifier for a specific decision",
                    "type": "string"
                },
                "dmnDecisionRequirementsName": {
                    "description": "the dmn name of the decision requirements, as parsed during deployment",
                    "type": "string"
                },
                "version": {
                    "description": "the assigned decision requirements version",
                    "type": "number"
                },
                "decisionRequirementsKey": {
                    "description": "the assigned decision requirements key, which acts as a unique identifier\nfor this decision requirements",
                    "type": "number"
                },
                "resourceName": {
                    "description": "the resource name (see: Resource.name) from which this decision\nrequirements was parsed",
                    "type": "string"
                }
            }
        }
    }
}
```


