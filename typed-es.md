# Typed ES (Stealify Lang)

## Faq

### How to create a optional parameter for a type
typeof NewType === { optStr?: string } via typeinference
```
const NewType = { 
  optStr: /** @type {string|undefined} */ ({}), 
};
```

most best do not create such types in general all Types Should result out of Function calls the Result of a Function call is the result of the Type

```js
const OtherTYpe = () => ''
//OtherType === string via typeinference
let me = OtherType(); // This knows me === string and nothing else!
```
