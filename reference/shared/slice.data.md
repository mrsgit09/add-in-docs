
# Slice.data property (JavaScript API for Office)
Gets the raw data of the file slice.

|||
|:-----|:-----|
|**Hosts:**|PowerPoint, Word|
|**Available in [Requirement set](http://msdn.microsoft.com/library/6b6702f2-b0a5-46ab-a356-8dda897ca8ae%28Office.15%29.aspx)**|File|
|**Last changed in**|1.1|

```
var sliceData = slice.data;
```


## Return value

The raw data of the file slice in  **Office.FileType.Text** ("text") or **Office.FileType.Compressed** ("compressed") format as specified by the _fileType_ parameter of the call to the [Document.getFileAsync](../../reference/shared/document.getfileasync.md) method.


## Remarks

Files in the "compressed" format will return a byte array that can be transformed to a base64-encoded string if required.


## Support details


A capital Y in the following matrix indicates that this property is supported in the corresponding Office host application. An empty cell indicates that the Office host application doesn't support this property.

For more information about Office host application and server requirements, see [Requirements for running Office Add-ins](http://msdn.microsoft.com/library/67340567-bb9a-498c-96d3-3f52f28c16bc%28Office.15%29.aspx).


||**Office for Windows desktop**|**Office Online(in browser)**|**Office for iPad**|
|:-----|:-----|:-----|:-----|
|**PowerPoint**|Y|Y|Y|
|**Word**|Y|Y|Y|


|||
|:-----|:-----|
|**Available in requirement sets**||
|**Minimum permission level**|[ReadDocument](http://msdn.microsoft.com/library/da2efadc-4ebf-45fe-be39-397ac1eb1dbd%28Office.15%29.aspx)|
|**Add-in types**|Content, task pane|
|**Library**|Office.js|
|**Namespace**|Office|

## Support history



****


|**Version**|**Changes**|
|:-----|:-----|
|1.1|Added support for PowerPoint and Word in Office for iPad.|
|1.0|Introduced|
