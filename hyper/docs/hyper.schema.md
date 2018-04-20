
# Example Hyper-Schema Schema

```
https://example.com/schemas/hyper
```

This is a *very* simple Example Hyper-Schema. There is only one property.

| Abstract | Extensible | Status | Custom Properties | Additional Properties | Defined In |
|----------|------------|--------|-------------------|-----------------------|------------|
| Can be instantiated | No | Experimental | Forbidden | Permitted | [hyper.schema.json](hyper.schema.json) |

# Example Hyper-Schema Links
| Name | Relation | href |
|------|----------|------|
| full | [full](#full) | `{id}` |
| author | [author](#author) | `/user?id={authorId}` |

## full


`full`
* rel: full
* href: `{id}`
* template parameters required:



## author


`author`
* rel: author
* href: `/user?id={authorId}`
* template parameters required:



# Example Hyper-Schema Properties

| Property | Type | Required | Defined by |
|----------|------|----------|------------|
| [authorId](#authorid) | `integer` | **Required** | Example Hyper-Schema (this schema) |
| [id](#id) | `number` | **Required** | Example Hyper-Schema (this schema) |
| [imgData](#imgdata) | `string` | Optional | Example Hyper-Schema (this schema) |
| [title](#title) | `string` | **Required** | Example Hyper-Schema (this schema) |
| `*` | any | Additional | this schema *allows* additional properties |

## authorId


`authorId`
* is **required**
* type: `integer`
* defined in this schema

### authorId Type


`integer`






## id
### Article Identifier

`id`
* is **required**
* type: `number`
* defined in this schema

### id Type


`number`






## imgData
### Article Illustration (small)

`imgData`
* is optional
* type: `string`
* defined in this schema

### imgData Type


`string`






## title
### Article Title

`title`
* is **required**
* type: `string`
* defined in this schema

### title Type


`string`





