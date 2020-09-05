# Node Ecosystem, TDD, CI/CD

### Description
- `Array.map()` to iterate of an array and return a new array with what you `return`
- `Array.reduce()` returned value is assigned to the accumulator, whose value is remembered across each iteration throughout the array, and ultimately becomes the final, single resulting value.


### superagent

#### as promise
```javascript
  superagent.get(url)
  .then((result) => {
    // code
  }).catch((err) => {
    // error
  })
```
#### as async function
```javascript
async getData(){
  try {
    const result = await superagent.get(url);    
    // code
  } catch (e) {
    // hanlde error
  }
}
```
