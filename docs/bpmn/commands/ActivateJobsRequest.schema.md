# 



<table>
<tbody>
<tr><th>$id</th><td>io.miranum.bpmn.command.v1.ActivateJobsRequest</td></tr>
<tr><th>$schema</th><td>http://json-schema.org/draft-07/schema#</td></tr>
</tbody>
</table>

## Properties

<table><thead><tr><th colspan="2">Name</th><th>Type</th></tr></thead><tbody><tr><td colspan="2"><a href="#type">type</a></td><td>String</td></tr><tr><td colspan="2"><a href="#worker">worker</a></td><td>String</td></tr><tr><td colspan="2"><a href="#timeout">timeout</a></td><td>Number</td></tr><tr><td colspan="2"><a href="#maxjobstoactivate">maxJobsToActivate</a></td><td>Number</td></tr><tr><td colspan="2"><a href="#fetchvariable">fetchVariable</a></td><td>Array</td></tr><tr><td colspan="2"><a href="#requesttimeout">requestTimeout</a></td><td>Number</td></tr></tbody></table>



<hr />



## type


<table>
  <tbody>
    <tr>
      <th>Description</th>
      <td colspan="2">the job type, as defined in the BPMN process</td>
    </tr>
    <tr><th>Type</th><td colspan="2">String</td></tr>
    <tr>
      <th>Required</th>
      <td colspan="2">No</td>
    </tr>
    
  </tbody>
</table>






## worker


<table>
  <tbody>
    <tr>
      <th>Description</th>
      <td colspan="2">the name of the worker activating the jobs, mostly used for logging purposes</td>
    </tr>
    <tr><th>Type</th><td colspan="2">String</td></tr>
    <tr>
      <th>Required</th>
      <td colspan="2">No</td>
    </tr>
    
  </tbody>
</table>






## timeout


<table>
  <tbody>
    <tr>
      <th>Description</th>
      <td colspan="2">a job returned after this call will not be activated by another call until the
timeout (in ms) has been reached</td>
    </tr>
    <tr><th>Type</th><td colspan="2">Number</td></tr>
    <tr>
      <th>Required</th>
      <td colspan="2">No</td>
    </tr>
    
  </tbody>
</table>






## maxJobsToActivate


<table>
  <tbody>
    <tr>
      <th>Description</th>
      <td colspan="2">the maximum jobs to activate by this request</td>
    </tr>
    <tr><th>Type</th><td colspan="2">Number</td></tr>
    <tr>
      <th>Required</th>
      <td colspan="2">No</td>
    </tr>
    
  </tbody>
</table>






## fetchVariable


<table>
  <tbody>
    <tr>
      <th>Description</th>
      <td colspan="2">a list of variables to fetch as the job variables; if empty, all visible variables at
the time of activation for the scope of the job will be returned</td>
    </tr>
    <tr><th>Type</th><td colspan="2">Array</td></tr>
    <tr>
      <th>Required</th>
      <td colspan="2">No</td>
    </tr>
    
  </tbody>
</table>






## requestTimeout


<table>
  <tbody>
    <tr>
      <th>Description</th>
      <td colspan="2">The request will be completed when at least one job is activated or after the requestTimeout (in ms).
if the requestTimeout &#x3D; 0, a default timeout is used.
if the requestTimeout &lt; 0, long polling is disabled and the request is completed immediately, even when no job is activated.</td>
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
    "$id": "io.miranum.bpmn.command.v1.ActivateJobsRequest",
    "$schema": "http://json-schema.org/draft-07/schema#",
    "type": "object",
    "properties": {
        "type": {
            "description": "the job type, as defined in the BPMN process",
            "type": "string"
        },
        "worker": {
            "description": "the name of the worker activating the jobs, mostly used for logging purposes",
            "type": "string"
        },
        "timeout": {
            "description": "a job returned after this call will not be activated by another call until the\ntimeout (in ms) has been reached",
            "type": "number"
        },
        "maxJobsToActivate": {
            "description": "the maximum jobs to activate by this request",
            "type": "number"
        },
        "fetchVariable": {
            "description": "a list of variables to fetch as the job variables; if empty, all visible variables at\nthe time of activation for the scope of the job will be returned",
            "type": "array",
            "items": {
                "type": "string"
            }
        },
        "requestTimeout": {
            "description": "The request will be completed when at least one job is activated or after the requestTimeout (in ms).\nif the requestTimeout = 0, a default timeout is used.\nif the requestTimeout < 0, long polling is disabled and the request is completed immediately, even when no job is activated.",
            "type": "number"
        }
    }
}
```


