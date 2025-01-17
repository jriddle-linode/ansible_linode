# account_availability_info

Get info about a Linode Account Availability.

- [Examples](#examples)
- [Parameters](#parameters)
- [Return Values](#return-values)

## Examples

```yaml
- name: Get info about the current Linode account availability
  linode.cloud.account_info: 
    region: us-east

```


## Parameters

| Field     | Type | Required | Description                                                                  |
|-----------|------|----------|------------------------------------------------------------------------------|
| `region` | <center>`str`</center> | <center>**Required**</center> | The Region of the Account Availability to resolve.   |

## Return Values

- `account_availability` - The returned Account Availability.

    - Sample Response:
        ```json
        
        {
          "region": "us-east",
          "unavailable": ["Linode"]
        }
        
        ```
    - See the [Linode API response documentation](TBD) for a list of returned fields


