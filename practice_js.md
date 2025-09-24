# Object Practice:
 ### max number with name

 ```javascript
let person={
  Ali:40,
  Ahmed:90,
  Bilal:34,
  Hassan:23
}
let topName = "";
let maxValue = -Infinity;

for (let key in person) {
  if (person[key] > maxValue) {
    maxValue = person[key];
    topName = key;
  }
}
delete maxValue.topName

console.log("Top Student:", topName, "Marks:", maxValue);
// Top Student: Ayesha Marks: 95

// console.log(maxperson) 
 ```

### => MAX number 

 ```javascript
let person={
  ali:40,
  ahmed:90,
  bilal:34,
  hassan:23
}
let maxperson=Math.max(...Object.values(person))
console.log(maxperson)
 ```
### => max number with name, topper number and name delete
``` let person={
 Ali:40,
 Ahmed:90,
 Bilal:34,
 Hassan:23
}
let topName = "";
let maxValue = -Infinity;

for (let key in person) {
 if (person[key] > maxValue) {
   maxValue = person[key];
   topName = key;
 }
}
delete person[topName]

console.log(person);
// Top Student: Ayesha Marks: 95

// console.log(maxperson) 
```
