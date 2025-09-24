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
```
### inventory in stock or not
``` let inventory = {pen: 10, pencil: 0, eraser: 5} 
for(let key in inventory){
  if(inventory[key]==0){
    console.log(key,"out of stock")
  }else{
    console.log(key, "In stock")
  }
}
```
### Ek object scores = {ali: 50, hassan: 85, hussain: 95} banao. If else ka use karke grades do:
90+ = A
70–89 = B
50–69 = C
below 50 = Fail
``` let scores = {ali: 50, hassan: 85, hussain: 95}
for (let name in scores) {
  let marks = scores[name];
if(marks>=90){
  console.log(marks,"grade A")
}else if( marks>=70 && marks<=89) {
  console.log(marks,"grade B")
}else if(marks>=50 && marks<=69){
  console.log(marks,"Grade C")
}else if(marks<50){
  console.log(marks,"Fail")
}
  
}
```
