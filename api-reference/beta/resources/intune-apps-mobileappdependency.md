---
title: "mobileAppDependency resource type"
description: "Describes a dependency type between two mobile apps."
author: "tfitzmac"
localization_priority: Normal
ms.prod: "Intune"
---

# mobileAppDependency resource type

> **Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.

> **Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.

Describes a dependency type between two mobile apps.


Inherits from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List mobileAppDependencies](../api/intune-apps-mobileappdependency-list.md)|[mobileAppDependency](../resources/intune-apps-mobileappdependency.md) collection|List properties and relationships of the [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) objects.|
|[Get mobileAppDependency](../api/intune-apps-mobileappdependency-get.md)|[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)|Read properties and relationships of the [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object.|
|[Create mobileAppDependency](../api/intune-apps-mobileappdependency-create.md)|[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)|Create a new [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object.|
|[Delete mobileAppDependency](../api/intune-apps-mobileappdependency-delete.md)|None|Deletes a [mobileAppDependency](../resources/intune-apps-mobileappdependency.md).|
|[Update mobileAppDependency](../api/intune-apps-mobileappdependency-update.md)|[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)|Update the properties of a [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|The relationship entity id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|
|targetId|String|The target child mobile app's app id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|
|targetDisplayName|String|The target child mobile app's display name. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|
|dependencyType|[mobileAppDependecyType](../resources/intune-apps-mobileappdependecytype.md)|The type of dependency relationship between the parent and child apps. Possible values are: `detect`, `autoInstall`.|
|dependentAppCount|Int32|The total number of dependencies the child app has.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppDependency"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppDependency",
  "id": "String (identifier)",
  "targetId": "String",
  "targetDisplayName": "String",
  "dependencyType": "String",
  "dependentAppCount": 1024
}
```





