

### Enumeration: FormAttachmentAssociationType
#### Enumerates the attachment association types. 

|Property | Value | Description | 
|---------|--------|--------|
| Any| 0| Any. 
| Exact| 1| Exact. 
| ExactOrNone| 2| ExactOrNone. 




## CIMFormAttachmentElement
#### Represents how one or more attachments can participate in the form. When present in the form, the user has the ability to upload an attachment specific to the form element. 


### CIMFormElement 

|Property | Type | Description | 
|---------|--------|--------|


### CIMFormAttachmentElement 

|Property | Type | Description | 
|---------|--------|--------|
| allowUserRename | boolean | A value indicating whether the user renaming an attachment is allowed. 
| attachmentKeyword | string | A string to identify the attachment(s). When a file is attached using the form, this property is used to set the value of the keywords field for the attachment. When a form is displaying existing attachments, this property is used to query attachments using an exact match on the keywords field. 
| description | string | A string that describes the element in detail. 
| displayFilename | boolean | A value indicating whether the file name should be displayed. Default is 'false'. 
| editableExpressionName | string | The name of an Arcade expression that returns a boolean value. When this expression evaluates to 'true', the element is editable. When the expression evaluates to 'false' the element is not editable. If set, this name must match the Name of exactly one expression in the form's ExpressionInfos array. 
| filenameExpression | string | An Arcade expression that is evaluated to produce filenames for new attachments. If not specified, a unique name will be generated using the 'AttachmentKeyword' and the current timestamp when the attachment is added. Unlike other uses of Arcade in forms, the value of this property is the expression to evaluate, not the name of an expression in the form's ExpressionInfos. 
| attachmentInput | [FormAttachmentInput](Types.md#formattachmentinput) | The input user interface to use for the attachment. 
| label | string | A string value indicating what the element represents. 
| maxAttachmentCount | long long | The maximum number of attachments allowed for this element. If set (or defaulted) to -1, there is no maximum. 
| minAttachmentCount | long long | The minimum number of attachments required for this element. If set (or defaulted) to 0, no attachements are required. 
| useOriginalFilename | boolean | A value indicating whether the uploaded attachment's file name is preserved. If 'false', the name is updated based on 'FilenameExpression'. Default is 'true'. 
| visibilityExpressionName | string | The name of an Arcade expression that returns a boolean value. When this expression evaluates to 'true', the element is displayed. When the expression evaluates to 'false' the element is not displayed. If no expression is provided, the default behavior is that the element is displayed. If set, this name must match the Name of exactly one expression in the form's ExpressionInfos array. 






## CIMFormAudioInput
#### Represents an attachment input that accepts audio files. 


### CIMFormAttachmentInput 

|Property | Type | Description | 
|---------|--------|--------|


### CIMFormAudioInput 

|Property | Type | Description | 
|---------|--------|--------|
| inputMethod | [enumeration FormElementInputMethod](CIMFormInfo.md#enumeration-formelementinputmethod) | The supported input methods used to attach an audio. 
| maxDuration | long long | The maximum length of an attachment for this element in seconds. If set (or defaulted) to -1, there is no maximum. 






## CIMFormBarcodeScannerInput
#### Represents a barcode or QR code scanner form input. If the client does not support barcode scanning, a single-line text box should be used. 


### CIMFormInput 

|Property | Type | Description | 
|---------|--------|--------|


### CIMFormBarcodeScannerInput 

|Property | Type | Description | 
|---------|--------|--------|
| maxLength | long long | The maximum number of characters allowed. This only applies for string fields. If set (or defaulted) to -1, the value is derived from the length property of the referenced field in the service. 
| minLength | long long | The minimum number of characters allowed. This only applies for string fields. If set (or defaulted) to 0, there is no minimum constraint. 






## CIMFormCodedValue
#### Represents a set of valid coded values with unique names. 


### CIMFormCodedValue 

|Property | Type | Description | 
|---------|--------|--------|
| codeAsDouble | double | The value stored in the feature attribute. 
| codeAsString | string | The value stored in the feature attribute. 
| name | string | The user-friendly name for what the code means. 






## CIMFormCodedValueDomain
#### Represents a coded value domain, which includes both the actual value that is stored in the database and the description of what the coded value means. 


### CIMFormDomain 

|Property | Type | Description | 
|---------|--------|--------|


### CIMFormCodedValueDomain 

|Property | Type | Description | 
|---------|--------|--------|
| codedValues | [[CIMFormCodedValue]](CIMFormInfo.md#cimformcodedvalue) | A set of valid values with unique names. 
| name | string | The domain name. 






## CIMFormComboBoxInput
#### Represents a form input consisting of a list of values in a drop-down that supports typing to filter. Only one value can be selected at a time. 


### CIMFormInput 

|Property | Type | Description | 
|---------|--------|--------|


### CIMFormComboBoxInput 

|Property | Type | Description | 
|---------|--------|--------|
| noValueOptionLabel | string | The text used to represent a null value. 
| showNoValueOption | boolean | A value indicating whether to display a null value option. If not provided, the default value is 'true'. 






## CIMFormDatePickerInput
#### Represents a date picker form input. 


### CIMFormInput 

|Property | Type | Description | 
|---------|--------|--------|


### CIMFormDatePickerInput 

|Property | Type | Description | 
|---------|--------|--------|
| max | [TimestampOffset](ExternalReferences.md#timestampoffset) | The maximum date to allow. Only the date portion of the timestamp is used. 
| min | [TimestampOffset](ExternalReferences.md#timestampoffset) | The minimum date to allow. Only the date portion of the timestamp is used. 






## CIMFormDatetimePickerInput
#### Represents a calendar date picker form input. 


### CIMFormInput 

|Property | Type | Description | 
|---------|--------|--------|


### CIMFormDatetimePickerInput 

|Property | Type | Description | 
|---------|--------|--------|
| includeTime | boolean | A value indicating whether the datetime picker should provide an option to select the time. If not provided, the default value is 'false'. 
| max | [TimestampOffset](ExternalReferences.md#timestampoffset) | The maximum date to allow. The offset of the timestamp is ignored. 
| min | [TimestampOffset](ExternalReferences.md#timestampoffset) | The minimum date to allow. The offset of the timestamp is ignored. 






## CIMFormDocumentInput
#### Represents an attachment input that accepts documents. 


### CIMFormAttachmentInput 

|Property | Type | Description | 
|---------|--------|--------|


### CIMFormDocumentInput 

|Property | Type | Description | 
|---------|--------|--------|
| maxFileSize | long long | The maximum size of an attachment for this element in bytes. If set (or defaulted) to -1, there is no maximum file size. 





### Enumeration: FormElementInputMethod
#### Enumerates the ways an element may acquire its value. 

|Property | Value | Description | 
|---------|--------|--------|
| Any| 0| Any. 
| Capture| 1| Capture. 
| Upload| 2| Upload. 




## CIMFormFieldElement
#### Represents how a field in the dataset participates in the form. 


### CIMFormElement 

|Property | Type | Description | 
|---------|--------|--------|


### CIMFormFieldElement 

|Property | Type | Description | 
|---------|--------|--------|
| description | string | A string that describes the element in detail. 
| domain | [FormDomain](Types.md#formdomain) | The domain to apply to this field. If defined, it takes precedence over domains defined in field, type, or subtype. 
| editableExpressionName | string | The name of an Arcade expression that returns a boolean value. When this expression evaluates to 'true', the element is editable. When the expression evaluates to 'false' the element is not editable. If the referenced field is not editable, the editable expression is ignored and the element is not editable. If set, this name must match the Name of exactly one expression in the form's ExpressionInfos array. 
| fieldName | string | A string containing the field name as defined by the layer or table. 
| hint | string | A string representing placeholder text. This only applies for input types that support text or numeric entry. 
| input | [FormInput](Types.md#forminput) | The input user interface to use for the element. 
| label | string | A string indicating what the element represents. If not supplied, the label is derived from the alias property in the referenced field in the service. 
| requiredExpressionName | string | The name of an Arcade expression that returns a boolean value. When this expression evaluates to 'true' and the element is visible, the element must have a valid value in order for the feature to be created or edited. When the expression evaluates to 'false' the element is not required. If no expression is provided, the default behavior is that the element is not required. If the referenced field is non-nullable, the required expression is ignored and the element is always required. If set, this name must match the Name of exactly one expression in the form's ExpressionInfos array. 
| valueExpressionName | string | The name of an Arcade expression that returns a date, number, or string value. When this expression evaluates the value of the field will be updated to the result. This expression is only evaluated when 'editableExpression' (if defined) is false but the field itself allows edits. If set, this name must match the Name of exactly one expression in the form's ExpressionInfos array. 
| visibilityExpressionName | string | The name of an Arcade expression that returns a boolean value. When this expression evaluates to 'true', the element is displayed. When the expression evaluates to 'false' the element is not displayed. If no expression is provided, the default behavior is that the element is displayed. Care must be taken when defining a visibility expression for a non-nullable field i.e. to make sure that such fields either have default values or are made visible to users so that they can provide a value before submitting the form. If set, this name must match the Name of exactly one expression in the form's ExpressionInfos array. 






## CIMFormGroupElement
#### Represents a container that holds a set of form elements that can be expanded, collapsed, or displayed together. 


### CIMFormElement 

|Property | Type | Description | 
|---------|--------|--------|


### CIMFormGroupElement 

|Property | Type | Description | 
|---------|--------|--------|
| description | string | A string that describes the element in detail. 
| formElements | [[CIMFormElement]](Types.md#formelement) | An array of Form Element objects that represent an ordered list of form elements. Nested group elements are not supported. 
| initialState | [enumeration FormGroupElementInitialState](CIMFormInfo.md#enumeration-formgroupelementinitialstate) | Whether the group should be expanded or collapsed when the form is initially displayed. If not provided, the default value is Expanded. 
| label | string | A string value indicating what the element represents. 
| visibilityExpressionName | string | The name of an Arcade expression that returns a boolean value. When this expression evaluates to 'true', the element is displayed. When the expression evaluates to 'false' the element is not displayed. If no expression is provided, the default behavior is that the element is displayed. If set, this name must match the Name of exactly one expression in the form's ExpressionInfos array. 





### Enumeration: FormGroupElementInitialState
#### Enumerates the initial states for group elements. 

|Property | Value | Description | 
|---------|--------|--------|
| Collapsed| 0| Collapsed. 
| Expanded| 1| Expanded. 




## CIMFormImageInput
#### Represents an attachment input that accepts image files. 


### CIMFormAttachmentInput 

|Property | Type | Description | 
|---------|--------|--------|


### CIMFormImageInput 

|Property | Type | Description | 
|---------|--------|--------|
| inputMethod | [enumeration FormElementInputMethod](CIMFormInfo.md#enumeration-formelementinputmethod) | The supported input methods used to attach an image. 
| maxImageSize | double | The number of pixels on the longest edge depending on orientation. Larger images will be resized and aspect ratio is maintained. If 'maxImageSize' is Double.NaN, images will not be resized. 






## CIMFormInfo
#### Represents the form configuration for when a user edits a feature. 


### CIMFormInfo 

|Property | Type | Description | 
|---------|--------|--------|
| description | string | A string that appears in the body of the form as a description. 
| expressionInfos | [[CIMExpressionInfo]](CIMRenderers.md#cimexpressioninfo) | The list of Arcade expressions used in the form. 
| formElements | [[CIMFormElement]](Types.md#formelement) | An array of formElement objects that represent an ordered list of form elements. 
| preserveFieldValuesWhenHidden | boolean | A value indicating whether a previously visible 'formFieldElement' value is retained or cleared when a 'visibilityExpression' applied on the 'formFieldElement' or its parent 'formGroupElement' evaluates to 'false'. Default is 'false'. 
| title | string | A string that appears at the top of the form as a title. 






## CIMFormInheritedDomain
#### Represents a domain inherited from the parent layer by a subtype. It implies that the domain for a field at the subtyp level is the same as the domain for the field at the layer level. 


### CIMFormDomain 

|Property | Type | Description | 
|---------|--------|--------|


### CIMFormInheritedDomain 

|Property | Type | Description | 
|---------|--------|--------|






## CIMFormRadioButtonsInput
#### Represents a radio button group form input. 


### CIMFormInput 

|Property | Type | Description | 
|---------|--------|--------|


### CIMFormRadioButtonsInput 

|Property | Type | Description | 
|---------|--------|--------|
| noValueOptionLabel | string | The text used to represent a null value. 
| showNoValueOption | boolean | A value indicating whether to display a null value option. If not provided, the default value is 'true'. 






## CIMFormRangeDomain
#### Represents a domain that specifies a range of valid values for a field. 


### CIMFormDomain 

|Property | Type | Description | 
|---------|--------|--------|


### CIMFormRangeDomain 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The domain name. 
| range | [double] | The range of valid values. The first element is the minValue and the second element is the maxValue. 





### Enumeration: FormRelationshipDisplayType
#### Enumerates the ways related records may be displayed. 

|Property | Value | Description | 
|---------|--------|--------|
| List| 0| List. 




## CIMFormRelationshipElement
#### Represents how a relationship between feature layers and tables can participate in the form. When present in the form, the user may have the option to add or edit related records. 


### CIMFormElement 

|Property | Type | Description | 
|---------|--------|--------|


### CIMFormRelationshipElement 

|Property | Type | Description | 
|---------|--------|--------|
| description | string | A string that describes the element in detail. 
| displayCount | long long | An integer that indicates the maximum number of records to display. If set (or defaulted) to -1, there is no maximum. 
| displayType | [enumeration FormRelationshipDisplayType](CIMFormInfo.md#enumeration-formrelationshipdisplaytype) | How related records should be displayed. 
| editableExpressionName | string | The name of an Arcade expression that returns a boolean value. When this expression evaluates to 'true', the element is editable. When the expression evaluates to 'false' the element is not editable. If the referenced related table is not editable, the editable expression is ignored and the element is not editable. If set, this name must match the Name of exactly one expression in the form's ExpressionInfos array. 
| label | string | A string value indicating what the element represents. 
| orderByFields | [[CIMFeatureSortInfo]](CIMVectorLayers.md#cimfeaturesortinfo) | The array of orderByField objects indicating the display order for the related records, and whether they should be sorted in ascending or descending order. 
| relationshipName | string | The name of the relationship as defined in the feature layer definition. 
| visibilityExpressionName | string | The name of an Arcade expression that returns a boolean value. When this expression evaluates to 'true', the element is displayed. When the expression evaluates to 'false' the element is not displayed. If no expression is provided, the default behavior is that the element is displayed. If set, this name must match the Name of exactly one expression in the form's ExpressionInfos array. 






## CIMFormSignatureInput
#### Represents an attachment input that captures and attaches signatures. 


### CIMFormAttachmentInput 

|Property | Type | Description | 
|---------|--------|--------|


### CIMFormSignatureInput 

|Property | Type | Description | 
|---------|--------|--------|
| inputMethod | [enumeration FormElementInputMethod](CIMFormInfo.md#enumeration-formelementinputmethod) | The supported input methods used to attach a signature. 






## CIMFormSupportedAttachmentsInput
#### Represents the kinds of supported files for attachment. 


### CIMFormAttachmentInput 

|Property | Type | Description | 
|---------|--------|--------|


### CIMFormSupportedAttachmentsInput 

|Property | Type | Description | 
|---------|--------|--------|
| attachmentAssociationType | [enumeration FormAttachmentAssociationType](CIMFormInfo.md#enumeration-formattachmentassociationtype) | Whether existing attachments should be associated with this element. 'Any' will associate all existing attachments to this form element; this can be the only 'formAttachmentElement' within the form. 'ExactOrNone' will associate any attachments with the associated 'keyword' and any attachments with no keyword defined; only one form element can have this value defined. 'Exact' will associate only attachments that include the specific keyword. 
| supportedInputs | [[CIMFormAttachmentInput]](Types.md#formattachmentinput) | The available inputs to add an attachment. (Nesting is not supported - CIMFormAttachmentInputs should not be added to this collection.) 






## CIMFormSwitchInput
#### Represents a binary switch, or toggle, form input. This should be used when selecting between two options. 


### CIMFormInput 

|Property | Type | Description | 
|---------|--------|--------|


### CIMFormSwitchInput 

|Property | Type | Description | 
|---------|--------|--------|
| offValueAsLong | long long | The coded value when switch state is 'off'. 
| offValueAsString | string | The coded value when switch state is 'off'. 
| onValueAsLong | long long | The coded value when switch state is 'on'. 
| onValueAsString | string | The coded value when switch state is 'on'. 






## CIMFormTextAreaInput
#### Represents a multi-line text area form input. 


### CIMFormInput 

|Property | Type | Description | 
|---------|--------|--------|


### CIMFormTextAreaInput 

|Property | Type | Description | 
|---------|--------|--------|
| maxLength | long long | The this represents the maximum number of characters allowed. If set (or defaulted) to -1, the value is derived from the length property of the referenced field in the service. 
| minLength | long long | The this represents the minimum number of characters allowed. If set (or defaulted) to 0, there is no minimum constraint. 






## CIMFormTextBoxInput
#### Represents a single-line text box form input. 


### CIMFormInput 

|Property | Type | Description | 
|---------|--------|--------|


### CIMFormTextBoxInput 

|Property | Type | Description | 
|---------|--------|--------|
| maxLength | long long | The maximum number of characters allowed. This only applies for string fields. If set (or defaulted) to -1, the value is derived from the length property of the referenced field in the service. 
| minLength | long long | The minimum number of characters allowed. This only applies for string fields. If set (or defaulted) to 0, there is no minimum constraint. 






## CIMFormTextElement
#### Represents a form element containing read-only text. 


### CIMFormElement 

|Property | Type | Description | 
|---------|--------|--------|


### CIMFormTextElement 

|Property | Type | Description | 
|---------|--------|--------|
| text | string | The string value indicating the text to be displayed within the formTextElement. 
| textFormat | [enumeration FormTextElementFormat](CIMFormInfo.md#enumeration-formtextelementformat) | The format of the 'text' property. Default is PlainText. 
| visibilityExpressionName | string | The name of an Arcade expression that returns a boolean value. When this expression evaluates to 'true', the element is displayed. When the expression evaluates to 'false' the element is not displayed. If no expression is provided, the default behavior is that the element is displayed. If set, this name must match the Name of exactly one expression in the form's ExpressionInfos array. 





### Enumeration: FormTextElementFormat
#### Enumerates the ways text may be formatted. 

|Property | Value | Description | 
|---------|--------|--------|
| Markdown| 0| Markdown. 
| PlainText| 1| PlainText. 




## CIMFormTimeInput
#### Represents a time picker form input. 


### CIMFormInput 

|Property | Type | Description | 
|---------|--------|--------|


### CIMFormTimeInput 

|Property | Type | Description | 
|---------|--------|--------|
| max | [TimestampOffset](ExternalReferences.md#timestampoffset) | The maximum time to allow. Only the time portion of the timestamp is used. 
| min | [TimestampOffset](ExternalReferences.md#timestampoffset) | The minimum time to allow. Only the time portion of the timestamp is used. 
| timeResolution | [enumeration FormTimeInputResolution](CIMFormInfo.md#enumeration-formtimeinputresolution) | The resolution identifier. The default value is Minutes. 





### Enumeration: FormTimeInputResolution
#### Enumerates time resolutions. 

|Property | Value | Description | 
|---------|--------|--------|
| Minutes| 0| Minutes. 
| Seconds| 1| Seconds. 




## CIMFormTimestampOffsetPickerInput
#### Reprsents calendar date and time picker, with time offset, form input. 


### CIMFormInput 

|Property | Type | Description | 
|---------|--------|--------|


### CIMFormTimestampOffsetPickerInput 

|Property | Type | Description | 
|---------|--------|--------|
| includeTimeOffset | boolean | A value indicating whether the timestampoffset picker should provide an option to select the timeoffset. If not provided, the default value is 'true'. 
| max | [TimestampOffset](ExternalReferences.md#timestampoffset) | The maximum timestampoffset to allow. 
| min | [TimestampOffset](ExternalReferences.md#timestampoffset) | The minimum timestampoffset to allow. 
| timeResolution | [enumeration FormTimeInputResolution](CIMFormInfo.md#enumeration-formtimeinputresolution) | The resolution identifier. The default value is Minutes. 






## CIMFormUtilityNetworkAssociationsElement
#### Represents how a utility network associations element can participate in the form. When present in the form, the user may have the option to view related utility network associations. 


### CIMFormElement 

|Property | Type | Description | 
|---------|--------|--------|


### CIMFormUtilityNetworkAssociationsElement 

|Property | Type | Description | 
|---------|--------|--------|
| associationTypes | [[CIMPopupUtilityNetworkAssociation]](CIMPopup.md#cimpopuputilitynetworkassociation) | The array of objects that define the type of associations to display in the pop-up. 
| description | string | A string that describes the element in detail. 
| editableExpressionName | string | The name of an Arcade expression that returns a boolean value. When this expression evaluates to 'true', the element is editable. When the expression evaluates to 'false' the element is not editable. If the referenced related table is not editable, the editable expression is ignored and the element is not editable. If set, this name must match the Name of exactly one expression in the form's ExpressionInfos array. 
| label | string | A string value indicating what the element represents. 
| visibilityExpressionName | string | The name of an Arcade expression that returns a boolean value. When this expression evaluates to 'true', the element is displayed. When the expression evaluates to 'false' the element is not displayed. If no expression is provided, the default behavior is that the element is displayed. If set, this name must match the Name of exactly one expression in the form's ExpressionInfos array. 






## CIMFormVideoInput
#### Represents an attachment input that accepts that a video file should be attached. 


### CIMFormAttachmentInput 

|Property | Type | Description | 
|---------|--------|--------|


### CIMFormVideoInput 

|Property | Type | Description | 
|---------|--------|--------|
| inputMethod | [enumeration FormElementInputMethod](CIMFormInfo.md#enumeration-formelementinputmethod) | The supported input methods used to attach a video. 
| maxDuration | long long | The defines the maximum length of an attachment for this element in seconds. If set (or defaulted) to -1, there is no maximum length. 



