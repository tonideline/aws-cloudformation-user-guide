# AWS::ServiceDiscovery::PrivateDnsNamespace<a name="aws-resource-servicediscovery-privatednsnamespace"></a>

The `AWS::ServiceDiscovery::PrivateDnsNamespace` resource specifies information about a private namespace for AWS Cloud Map\. Use a private namespace when you want to route traffic inside an Amazon VPC\. For more information, see [CreatePrivateDnsNamespace](https://docs.aws.amazon.com/cloud-map/latest/api/API_CreatePrivateDnsNamespace.html) in the *AWS Cloud Map API Reference*\.

**Topics**
+ [Syntax](#aws-resource-servicediscovery-privatednsnamespace-syntax)
+ [Properties](#aws-resource-servicediscovery-privatednsnamespace-properties)
+ [Return Values](#aws-resource-servicediscovery-privatednsnamespace-returnvalues)
+ [See Also](#aws-resource-servicediscovery-privatednsnamespace-seealso)

## Syntax<a name="aws-resource-servicediscovery-privatednsnamespace-syntax"></a>

To declare this entity in your AWS CloudFormation template, use the following syntax:

### JSON<a name="aws-resource-servicediscovery-privatednsnamespace-syntax.json"></a>

```
{
  "Type" : "AWS::ServiceDiscovery::PrivateDnsNamespace",
  "Properties" : {
    "[Description](#cfn-servicediscovery-privatednsnamespace-description)" : String,
    "[Vpc](#cfn-servicediscovery-privatednsnamespace-vpc)" : String,
    "[Name](#cfn-servicediscovery-privatednsnamespace-name)" : String
  }
}
```

### YAML<a name="aws-resource-servicediscovery-privatednsnamespace-syntax.yaml"></a>

```
Type: "AWS::ServiceDiscovery::PrivateDnsNamespace"
Properties:
  [Description](#cfn-servicediscovery-privatednsnamespace-description): String
  [Vpc](#cfn-servicediscovery-privatednsnamespace-vpc): String
  [Name](#cfn-servicediscovery-privatednsnamespace-name): String
```

## Properties<a name="aws-resource-servicediscovery-privatednsnamespace-properties"></a>

`Description`  <a name="cfn-servicediscovery-privatednsnamespace-description"></a>
A description for the namespace\.  
*Required*: No  
*Type*: String  
*Update requires*: [Replacement](using-cfn-updating-stacks-update-behaviors.md#update-replacement)

`Vpc`  <a name="cfn-servicediscovery-privatednsnamespace-vpc"></a>
The ID of the Amazon VPC that you want to associate the namespace with\.  
*Required*: Yes  
*Type*: String  
*Update requires*: [Replacement](using-cfn-updating-stacks-update-behaviors.md#update-replacement)

`Name`  <a name="cfn-servicediscovery-privatednsnamespace-name"></a>
The name that you want to assign to this namespace\. When you create a namespace, AWS Cloud Map automatically creates a hosted zone that has the same name as the namespace\.  
*Required*: Yes  
*Type*: String  
*Update requires*: [Replacement](using-cfn-updating-stacks-update-behaviors.md#update-replacement)

## Return Values<a name="aws-resource-servicediscovery-privatednsnamespace-returnvalues"></a>

### Ref<a name="aws-resource-servicediscovery-privatednsnamespace-ref"></a>

When you pass the logical ID of an `AWS::ServiceDiscovery::PrivateDnsNamespace` resource to the intrinsic `Ref` function, the function returns the value of `Id` for the namespace\.

For more information about using the `Ref` function, see [Ref](intrinsic-function-reference-ref.md)\.

### Fn::GetAtt<a name="aws-resource-servicediscovery-privatednsnamespace-getatt"></a>

`Fn::GetAtt` returns a value for a specified attribute of this type\. The following are the available attributes and sample return values\.

`Id`  
The ID of the private namespace\.

`Arn`  
The Amazon Resource Name \(ARN\) of the private namespace\.

For more information about using `Fn::GetAtt`, see [Fn::GetAtt](intrinsic-function-reference-getatt.md)\.

## See Also<a name="aws-resource-servicediscovery-privatednsnamespace-seealso"></a>
+ [CreatePrivateDnsNamespace](https://docs.aws.amazon.com/cloud-map/latest/api/API_CreatePrivateDnsNamespace.html) in the *AWS Cloud Map API Reference*