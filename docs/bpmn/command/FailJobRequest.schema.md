# 



<table>
<tbody>
<tr><th>$id</th><td>io.miranum.bpmn.command.v1.FailJobRequest</td></tr>
<tr><th>$schema</th><td>http://json-schema.org/draft-07/schema#</td></tr>
</tbody>
</table>

## Properties

<table><thead><tr><th colspan="2">Name</th><th>Type</th></tr></thead><tbody><tr><td colspan="2"><a href="#jobkey">jobKey</a></td><td>Number</td></tr><tr><td colspan="2"><a href="#retries">retries</a></td><td>Number</td></tr><tr><td colspan="2"><a href="#errormessage">errorMessage</a></td><td>String</td></tr><tr><td colspan="2"><a href="#retrybackoff">retryBackOff</a></td><td>Number</td></tr><tr><td colspan="2"><a href="#variables">variables</a></td><td>String</td></tr></tbody></table>



<hr />



## jobKey


<table>
  <tbody>
    <tr>
      <th>Description</th>
      <td colspan="2">the unique job identifier, as obtained when activating the job</td>
    </tr>
    <tr><th>Type</th><td colspan="2">Number</td></tr>
    <tr>
      <th>Required</th>
      <td colspan="2">No</td>
    </tr>
    
  </tbody>
</table>






## retries


<table>
  <tbody>
    <tr>
      <th>Description</th>
      <td colspan="2">the amount of retries the job should have left</td>
    </tr>
    <tr><th>Type</th><td colspan="2">Number</td></tr>
    <tr>
      <th>Required</th>
      <td colspan="2">No</td>
    </tr>
    
  </tbody>
</table>






## errorMessage


<table>
  <tbody>
    <tr>
      <th>Description</th>
      <td colspan="2">an optional message describing why the job failed
this is particularly useful if a job runs out of retries and an incident is raised,
as it this message can help explain why an incident was raised</td>
    </tr>
    <tr><th>Type</th><td colspan="2">String</td></tr>
    <tr>
      <th>Required</th>
      <td colspan="2">No</td>
    </tr>
    
  </tbody>
</table>






## retryBackOff


<table>
  <tbody>
    <tr>
      <th>Description</th>
      <td colspan="2">the backoff timeout (in ms) for the next retry</td>
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
      <td colspan="2">JSON document that will instantiate the variables at the local scope of the
job&#x27;s associated task; it must be a JSON object, as variables will be mapped in a
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










<hr />

## Schema
```
{
    "$id": "io.miranum.bpmn.command.v1.FailJobRequest",
    "$schema": "http://json-schema.org/draft-07/schema#",
    "type": "object",
    "properties": {
        "jobKey": {
            "description": "the unique job identifier, as obtained when activating the job",
            "type": "number"
        },
        "retries": {
            "description": "the amount of retries the job should have left",
            "type": "number"
        },
        "errorMessage": {
            "description": "an optional message describing why the job failed\nthis is particularly useful if a job runs out of retries and an incident is raised,\nas it this message can help explain why an incident was raised",
            "type": "string"
        },
        "retryBackOff": {
            "description": "the backoff timeout (in ms) for the next retry",
            "type": "number"
        },
        "variables": {
            "description": "JSON document that will instantiate the variables at the local scope of the\njob's associated task; it must be a JSON object, as variables will be mapped in a\nkey-value fashion. e.g. { \"a\": 1, \"b\": 2 } will create two variables, named \"a\" and\n\"b\" respectively, with their associated values. [{ \"a\": 1, \"b\": 2 }] would not be a\nvalid argument, as the root of the JSON document is an array and not an object.",
            "type": "string"
        }
    }
}
```


