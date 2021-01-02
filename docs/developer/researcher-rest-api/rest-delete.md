
Delete one or more Run:AI Jobs.

## General

__URL__:  `http://<service-url>/api/job`

__Method__: `DELETE`

## Request 

Following JSON:

```
[<Job Identifier 1>, .... ,<Job Identifier n>]
```

Job identifier definition:

``` json
{
    "name": "<job-name>", 
    "project": "<job-project>"
}
```

    
## Examples

``` bash
curl --location --request DELETE 'http://example.com/api/job' \
--header 'Content-Type: application/json' \
--data-raw '[
    {"name" : "job-name-0", "project" : "team-a"}, 
    {"name" : "job-name-1", "project" : "team-a"}
]'
```