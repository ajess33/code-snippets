# Code-Snippets
Code I find myself having to search Google for more than once, all in one place.

### JavaScript
**Dynamically add properties to an object**
```
const { firstName, lastName, address, age } = person

const dynamicObject = {
  ...(firstName && { firstName }),
  ...(lastName && { lastName }),
  ...(address.length === 3 && { address }),
  ...(age && { age })
}
```
