# JSON Patch

JSON Patch is a format to describe changes to a JSON document. It can be used along with a HTTP [[PATCH]] request to allow partial updates. Its useful when you only have to update few fields in the document and don't want to send the complete document.

## Escaping JSON Patch Payload

- `~` is encoded as `~0`
- `/` is encoded as `~1`

## References

- [JSONPatch.com](https://jsonpatch.com/)
- [Escape JSON Patch Path for Key with Backslash - Github Issues - json-patch-tests](https://github.com/json-patch/json-patch-tests/issues/42)
- [RFC6901,section 3](https://tools.ietf.org/html/rfc6901#section-3)
