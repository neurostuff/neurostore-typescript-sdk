# ConditionRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **string** | Name of the condition being applied in the contrast, either psychological, pharmacological, or group based. | [optional] [default to undefined]
**description** | **string** | Long form description of how the condition is operationalized and/or specific meaning. | [optional] [default to undefined]
**id** | **string** | short UUID specifying the location of this resource | [optional] [default to undefined]
**_public** | **boolean** | whether the resource is listed in public searches or not | [optional] [default to true]

## Example

```typescript
import { ConditionRequest } from './api';

const instance: ConditionRequest = {
    name,
    description,
    id,
    _public,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
