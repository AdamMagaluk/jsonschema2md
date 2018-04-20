
#  Schema

```
https://schema.example.com/thing-collection
```


| Abstract | Extensible | Status | Custom Properties | Additional Properties | Defined In |
|----------|------------|--------|-------------------|-----------------------|------------|
| Can be instantiated | No | Experimental | Forbidden | Permitted | [collection.schema.json](collection.schema.json) |

#  Links
| Name | Relation | href |
|------|----------|------|
| self | [self](#self) | `things` |

## self


`self`
* rel: self
* href: `things`
* template parameters required:




#  Properties

| Property | Type | Required | Defined by |
|----------|------|----------|------------|
| [elements](#elements) | `array` | **Required** |  (this schema) |
| `*` | any | Additional | this schema *allows* additional properties |

## elements


`elements`
* is **required**
* type: `array`

* defined in this schema

### elements Type


Array type: `array`

All items must be of the type:
Unknown type ``.

```json
{
  "type": "array",
  "items": {
    "allOf": [
      {
        "$ref": "thing#"
      }
    ],
    "links": [
      {
        "anchorPointer": "",
        "rel": "item",
        "href": "things/{id}",
        "templateRequired": [
          "id"
        ],
        "targetSchema": {
          "$ref": "thing#"
        }
      }
    ],
    "simpletype": "complex"
  },
  "isrequired": true,
  "simpletype": "`array`"
}
```







