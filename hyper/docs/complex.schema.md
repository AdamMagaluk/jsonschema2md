
# Sample File System Storage Schema Schema

```
https://2018.restfest.org/midwest/schemas/fs-schema#
```

schema for an fstab entry

| Abstract | Extensible | Status | Custom Properties | Additional Properties | Defined In |
|----------|------------|--------|-------------------|-----------------------|------------|
| Can be instantiated | Yes | Experimental | Forbidden | Permitted | [complex.schema.json](complex.schema.json) |

# Sample File System Storage Schema Links
| Name | Relation | href |
|------|----------|------|
| item | [item](#item) | `/disk/{diskid}` |

## item


`item`
* rel: item
* href: `/disk/{diskid}`
* template parameters required:



# Sample File System Storage Schema Properties

| Property | Type | Required | Defined by |
|----------|------|----------|------------|
| [diskid](#diskid) | `string` | Optional | Sample File System Storage Schema (this schema) |
| [fstype](#fstype) | `enum` | Optional | Sample File System Storage Schema (this schema) |
| [options](#options) | `string[]` | Optional | Sample File System Storage Schema (this schema) |
| [readonly](#readonly) | `boolean` | Optional | Sample File System Storage Schema (this schema) |
| [storage](#storage) | `object` | **Required** | Sample File System Storage Schema (this schema) |
| `*` | any | Additional | this schema *allows* additional properties |

## diskid


`diskid`
* is optional
* type: `string`
* defined in this schema

### diskid Type


`string`






## fstype


`fstype`
* is optional
* type: `enum`
* defined in this schema

The value of this property **must** be equal to one of the [known values below](#fstype-known-values).

### fstype Known Values
| Value | Description |
|-------|-------------|
| `ext3` |  |
| `ext4` |  |
| `btrfs` |  |




## options


`options`
* is optional
* type: `string[]`
* at least `1` items in the array
* defined in this schema

### options Type


Array type: `string[]`

All items must be of the type:
`string`









## readonly


`readonly`
* is optional
* type: `boolean`
* defined in this schema

### readonly Type


`boolean`





## storage


`storage`
* is **required**
* type: `object`
* defined in this schema

### storage Type


`object` with following properties:


| Property | Type | Required
|----------|------|----------|
| `id`| string | **Required** | 
| `remotePath`| string | **Required** | 
| `server`| string | **Required** | 
| `type`|  | **Required** | 



#### id

undefined

`id`
* is **required**
* type: `string`

##### id Type


`string`








#### remotePath

undefined

`remotePath`
* is **required**
* type: `string`

##### remotePath Type


`string`


All instances must conform to this regular expression 
(test examples [here](https://regexr.com/?expression=%5E(%2F%5B%5E%2F%5D%2B)%2B%24)):
```regex
^(/[^/]+)+$
```








#### server

undefined

`server`
* is **required**
* type: `string`

##### server Type


`string`








#### type

undefined

`type`
* is **required**
* type: `undefined`

The value of this property **must** be equal to one of the [known values below](#type-known-values).

##### type Known Values
| Value | Description |
|-------|-------------|









# Sample File System Storage Schema Definitions

| Property | Type | Group |
|----------|------|-------|
| [device](#device) | `string` | `https://2018.restfest.org/midwest/schemas/fs-schema##/definitions/diskDevice` |
| [id](#id) | `string` | `https://2018.restfest.org/midwest/schemas/fs-schema##/definitions/nfs` |
| [label](#label) | `string` | `https://2018.restfest.org/midwest/schemas/fs-schema##/definitions/diskUUID` |
| [remotePath](#remotepath) | `string` | `https://2018.restfest.org/midwest/schemas/fs-schema##/definitions/nfs` |
| [server](#server) | `string` | `https://2018.restfest.org/midwest/schemas/fs-schema##/definitions/nfs` |
| [sizeInMB](#sizeinmb) | `integer` | `https://2018.restfest.org/midwest/schemas/fs-schema##/definitions/tmpfs` |
| [type](#type) | `enum` | `https://2018.restfest.org/midwest/schemas/fs-schema##/definitions/tmpfs` |

## device


`device`
* is optional
* type: `string`
* defined in this schema

### device Type


`string`


All instances must conform to this regular expression 
(test examples [here](https://regexr.com/?expression=%5E%2Fdev%2F%5B%5E%2F%5D%2B(%2F%5B%5E%2F%5D%2B)*%24)):
```regex
^/dev/[^/]+(/[^/]+)*$
```






## id


`id`
* is optional
* type: `string`
* defined in this schema

### id Type


`string`






## label


`label`
* is optional
* type: `string`
* defined in this schema

### label Type


`string`


All instances must conform to this regular expression 
(test examples [here](https://regexr.com/?expression=%5E%5Ba-fA-F0-9%5D%7B8%7D-%5Ba-fA-F0-9%5D%7B4%7D-%5Ba-fA-F0-9%5D%7B4%7D-%5Ba-fA-F0-9%5D%7B4%7D-%5Ba-fA-F0-9%5D%7B12%7D%24)):
```regex
^[a-fA-F0-9]{8}-[a-fA-F0-9]{4}-[a-fA-F0-9]{4}-[a-fA-F0-9]{4}-[a-fA-F0-9]{12}$
```






## remotePath


`remotePath`
* is optional
* type: `string`
* defined in this schema

### remotePath Type


`string`


All instances must conform to this regular expression 
(test examples [here](https://regexr.com/?expression=%5E(%2F%5B%5E%2F%5D%2B)%2B%24)):
```regex
^(/[^/]+)+$
```






## server


`server`
* is optional
* type: `string`
* defined in this schema

### server Type


`string`






## sizeInMB


`sizeInMB`
* is optional
* type: `integer`
* defined in this schema

### sizeInMB Type


`integer`
* minimum value: `16`
* maximum value: `512`





## type


`type`
* is optional
* type: `enum`
* defined in this schema

The value of this property **must** be equal to one of the [known values below](#type-known-values).

### type Known Values
| Value | Description |
|-------|-------------|
| `tmpfs` |  |



