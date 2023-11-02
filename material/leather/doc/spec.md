<!-- 10-Header -->
Entity: leather  
===============
<!-- 15-License -->


<!-- /15-License -->
<!-- 20-Description -->


<!-- /20-Description -->
<!-- 30-PropertiesList -->




- `address[object]`: The mailing address  . Model: [https://schema.org/address](https://schema.org/address)
	- `addressLocality[string]`: Property. The locality in which the street address is, and which is in the region. Model:'https://schema.org/addressLocality'    
	- `addressRegion[string]`: Property. The region in which the locality is, and which is in the country. Model:'https://schema.org/addressRegion'    
	- `district[string]`: Property. A district is a type of administrative division that, in some countries, is managed by the local government    
	- `postOfficeBoxNumber[string]`: Property. The post office box number for PO box addresses. For example, 03578. Model:'https://schema.org/postOfficeBoxNumber'    
	- `postalCode[string]`: Property. The postal code. For example, 24004. Model:'https://schema.org/https://schema.org/postalCode'    
	- `streetAddress[string]`: Property. The street address. Model:'https://schema.org/streetAddress'    
	- `streetNr[string]`: Property. Number identifying a specific property on a public street    
- `alternateName[string]`: An alternative name for this item  
<!-- 35-RequiredProperties -->

- `color`  
<!-- 40-RequiredProperties -->
<!-- /40-RequiredProperties -->
<!-- 50-DataModelHeader -->


<!-- /50-DataModelHeader -->
<!-- 60-ModelYaml -->
<details><summary><strong>full yaml details</strong></summary>    

leather:    
  description: Representing leather material for the CIRCILOOS project    
  properties:    
    address:    
      description: The mailing address    
      properties:    
        addressCountry:    
          description: Property. The country. For example, Spain. Model:'https://schema.org/addressCountry'    
          type: string    
        addressLocality:    
          description: Property. The locality in which the street address is, and which is in the region. Model:'https://schema.org/addressLocality'    
          type: string    
        addressRegion:    
          description: Property. The region in which the locality is, and which is in the country. Model:'https://schema.org/addressRegion'    
          type: string    
        district:    
          description: Property. A district is a type of administrative division that, in some countries, is managed by the local government    
          type: string    
        postOfficeBoxNumber:    
          description: Property. The post office box number for PO box addresses. For example, 03578. Model:'https://schema.org/postOfficeBoxNumber'    
          type: string    
        postalCode:    
          description: Property. The postal code. For example, 24004. Model:'https://schema.org/https://schema.org/postalCode'    
          type: string    
        streetAddress:    
          description: Property. The street address. Model:'https://schema.org/streetAddress'    
          type: string    
        streetNr:    
          description: Property. Number identifying a specific property on a public street    
          type: string    
      type: object    
      x-ngsi:    
        model: https://schema.org/address    
        type: Property    
    alternateName:    
      description: An alternative name for this item    
      type: string    
      x-ngsi:    
        type: Property    
    areaServed:    
      description: The geographic area where a service or offered item is provided    
      type: string    
      x-ngsi:    
        model: https://schema.org/Text    
        type: Property    
    color:    
      description: The final color of the leather    
      enum:    
        - brown    
        - black    
        - '....'    
        - rainbow    
      type: string    
      x-ngsi:    
        type: Property    
    dataProvider:    
      description: A sequence of characters identifying the provider of the harmonised data entity    
      type: string    
      x-ngsi:    
        type: Property    
    dateCreated:    
      description: Entity creation timestamp. This will usually be allocated by the storage platform    
      format: date-time    
      type: string    
      x-ngsi:    
        type: Property    
    dateModified:    
      description: Timestamp of the last modification of the entity. This will usually be allocated by the storage platform    
      format: date-time    
      type: string    
      x-ngsi:    
        type: Property    
    description:    
      description: A description of this item    
      type: string    
      x-ngsi:    
        type: Property    
    hardness:    
      description: Overall hardness of the leather    
      enum:    
        - soft    
        - medium    
        - hard    
      type: string    
      x-ngsi:    
        type: Property    
    id:    
      anyOf:    
        - description: Property. Identifier format of any NGSI entity    
          maxLength: 256    
          minLength: 1    
          pattern: ^[\w\-\.\{\}\$\+\*\[\]`|~^@!,:\\]+$    
          type: string    
        - description: Property. Identifier format of any NGSI entity    
          format: uri    
          type: string    
      description: Unique identifier of the entity    
      x-ngsi:    
        type: Property    
    origin:    
      description: The source that the leather was originated    
      enum:    
        - cow    
        - pig    
        - horse    
        - other animals    
        - vegan    
      type: string    
      x-ngsi:    
        type: Property    
    owner:    
      description: A List containing a JSON encoded sequence of characters referencing the unique Ids of the owner(s)    
      items:    
        anyOf:    
          - description: Property. Identifier format of any NGSI entity    
            maxLength: 256    
            minLength: 1    
            pattern: ^[\w\-\.\{\}\$\+\*\[\]`|~^@!,:\\]+$    
            type: string    
          - description: Property. Identifier format of any NGSI entity    
            format: uri    
            type: string    
        description: Property. Unique identifier of the entity    
      type: array    
      x-ngsi:    
        type: Property    
    recycledTimes:    
      description: The number of times that the leather have been recycled    
      minimum: 0    
      type: integer    
      x-ngsi:    
        type: Property    
    seeAlso:    
      description: list of uri pointing to additional resources about the item    
      oneOf:    
        - items:    
            format: uri    
            type: string    
          minItems: 1    
          type: array    
        - format: uri    
          type: string    
      x-ngsi:    
        type: Property    
    source:    
      description: A sequence of characters giving the original source of the entity data as a URL. Recommended to be the fully qualified domain name of the source provider, or the URL to the source object    
      type: string    
      x-ngsi:    
        type: Property    
    surfaceFinishWithCovering:    
      description: Leather finished (with covering) or not finished    
      type: boolean    
      x-ngsi:    
        type: Property    
    surfaceSize:    
      description: The surface size of the leather. Unit palm ie humman palm    
      minimum: 0    
      type: integer    
      x-ngsi:    
        type: Property    
    tannedProcess:    
      description: The tanned used    
      enum:    
        - chrome    
        - vegetable    
      type: string    
      x-ngsi:    
        type: Property    
    thickness:    
      description: The thickness of the leather    
      minimum: 0    
      type: float    
      x-ngsi:    
        type: Property    
    type:    
      description: NGSI Entity type. It has to be Storey, leather    
      enum:    
        - leather    
      type: string    
      x-ngsi:    
        type: Property    
    type1:    
      description: The treatment used    
      enum:    
        - grainside    
        - split    
        - nubuck    
        - suede    
        - furs    
      type: string    
      x-ngsi:    
        type: Property    
  required:    
    - id    
    - type    
    - color    
    - surfaceSize    
  type: object    
  x-derived-from: ''    
  x-disclaimer: Redistribution and use in source and binary forms, with or without modification, are permitted  provided that the license conditions are met. Copyleft (c) 2021 Contributors to Smart Data Models Program    
  x-license-url: https://github.com/smart-data-models/circuloos_data_model/blob/master/leather/LICENSE.md    
  x-model-schema: https://raw.githubusercontent.com/TO_ADD_LATER/schema.json    
  x-model-tags: ''    
  x-version: 0.0.1    
```  
</details>    
<!-- /60-ModelYaml -->
<!-- 70-MiddleNotes -->
<!-- /70-MiddleNotes -->
<!-- 80-Examples -->




<details><summary><strong>show/hide example</strong></summary>    


    "id": "urn:ngsi-ld:leather:IDAS1313",  
    "type": "leather",  
    "origin": {  
        "type": "Property",  
        "value": "vegan"  
    },  
    "color": {  
        "type": "Property",  
        "value": "black"  
    },  
    "surfaceSize": {  
        "type": "Property",  
        "value": "2"  
    },  
    "thickness": {  
        "type": "Property",  
        "value": "0.3",  
        "unitCode": "MMT"  
    },  
    "tannedProcess": {  
        "type": "Property",  
        "value": "vegetable"  
    },  
    "type1": {  
        "type": "Property",  
        "value": "split"  
    },  
    "surfaceFinishWithCovering": {  
        "type": "Property",  
        "value": "true"  
    },  
    "hardness": {  
        "type": "Property",  
        "value": "medium"  
    },  
    "recycledTimes": {  
        "type": "Property",  
        "value": "2"  
    },  
     "@context": [  
        "https://TOBELater/context.jsonld"  
    ]  
}  
```  
</details><!-- /80-Examples -->