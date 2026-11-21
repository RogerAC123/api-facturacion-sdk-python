# UploadCompanyCertificateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | 
**password** | **str** |  | 
**content** | **str** | Base64 del .p12/.pfx | 

## Example

```python
from intifact_sdk.models.upload_company_certificate_request import UploadCompanyCertificateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of UploadCompanyCertificateRequest from a JSON string
upload_company_certificate_request_instance = UploadCompanyCertificateRequest.from_json(json)
# print the JSON string representation of the object
print(UploadCompanyCertificateRequest.to_json())

# convert the object into a dict
upload_company_certificate_request_dict = upload_company_certificate_request_instance.to_dict()
# create an instance of UploadCompanyCertificateRequest from a dict
upload_company_certificate_request_from_dict = UploadCompanyCertificateRequest.from_dict(upload_company_certificate_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


