# JSQuiz

##  13. How to find duplicate elements in a given array?
```javascript
let Check=(arr)=>{
    console.log(arr.sort());
    let set=new Set()
    for(let i =0; i<arr.length;i++){
        for(let j=i+1; j<arr.length;j++){
            if(arr[i]== arr[j]){
                set.add(arr[j])
            }
        }
    }
    return set
}
console.log([...Check([1,2,3,4,5,1,10,2,6,6,4,7,3])])
```
##  14. "How to find the unique value from an array in sorted order?


```javascript
let Check=(arr)=>{
    return [...new Set(arr.sort())]
}
console.log([...Check([23,25,23, 45, 34, 33, 87, 45, 76, 25])])
```


## 15. "Write a code to create a sentence from the given array?
```javascript
let arr = ["Hi", "I am", "Full Stack" , "Developer"]
console.log(arr.join(' '))
 ```
## 16.  Given a two strings find out if they are anagram of each other
```javascript 
let check=(a,b)=>{
    let val1 = a.split('').sort().join('');
    let val2 = b.split('').sort().join('');
    if(a.length===b.length){
        if(val1===val2){
            return true
        }else{
            return false
        }
    }else{
        return false
    }

}
console.log(check("lol","lol"))
```
## 17.  How can you extract  a few fields  from the given JSON object  and form a new array? 
```javascript
const input = {
    "students" : [
        {
        name : "Ravi",
        id: 10
        },
        {
        name : "Mahesh",
        id: 6
        },
        {
        name : "Surya",
        id: 7
        }]
 }
console.log([input.students[0],input.students[1]])
```
## 18. "Tell me the output of this code : 
```javascript 
const a = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10];

for (let i = 0; i < 10; i++) {
  setTimeout(() => console.log(a[i]), 1000);
}
for (var i = 0; i < 10; i++) {
  setTimeout(() => console.log(a[i]), 1000);
}
// print 1 to 10  after that 10 times undefined
```

## 19. How to convert an Object {} into an Array [] in JavaScript?

```javascript
 let arr=[]
let obj={
    name:"Arjun",
}
arr.push(obj)
console.log(arr)

// or

let obj =  {
    name : "Arjun"
}
console.log(Object.entries(obj));

```

## 20. Write a function that takes an array of numbers and returns the median value.
```javascript
let mean=(arr)=>{
    let data=0
    for(let i=0;i<arr.length;i++){
        data+=arr[i]
    }
    return data/arr.length
}
console.log(mean([123,232,323,434,235,16,327,128,139]))


let median=(arr)=>{
    let data=arr.sort()
    value=Math.floor(data.length/2)
    if(arr.length%2===0){
        return (data[value]+data[value-1])/2
    }else{
        return (data[value])
    }
}
console.log(median([12,23,32,44,23,16,20,15,32,18,19,10]))
```
## 21. Output Based Question:
```javascript
var Employee = { company: "abc" };
var emp1 = Object.create(Employee);
delete emp1.company
console.log(emp1.company); 

// Output : abc
```

##  22.  How do you check whether a string contains a substring
```javascript
 console.log(string.includes("Hello"))
 let string="Hello Brother!"
let check=(data)=>{
    let arr=string.split(" ")
    for(let i=0;i<arr.length;i++){
        if(arr[i]===data){
            return true
        }else{
            return false
        }
    }
}
console.log(check('Helo'))
 ```
 ## 23. Create a function that will convert from Celsius to Fahrenheit
 ```javascript
 let temp=(n)=>{
    return (n*(9/5))+32
}
console.log(`${temp(10)}F`)
```
## 24. Create a function that will find the nth Fibonacci number using recursion
```javascript
let FibonacciCheck=(arr)=>{
    let count=0
    for(let i=0;i<arr.length;i++){
        if(arr[i]+arr[i+1]==arr[i+2]){
            count++
        }
    }
    if((arr.length-2)==count){
        return true
    }else{
        return false
    }
}
console.log(FibonacciCheck([0,1,1,2,3,5,8]))
```

## 25. Create a function that will receive two arrays of numbers as arguments and return an array composed of all the numbers that are either in the first array or second array but not in both
 
```javascript

let a=[1,2,3,4,5,6]
let b=[6,7,8,9,10]
let check=(a,b)=>{
    let c=new Set([...a,...b])
    return [...c]
}

console.log(check(a,b))
```
##  26. Create a function to return the longest word from the string let text = ""Create a function to return the longest word(s) in a sentance
```javascript
let CheckString=(str)=>{
    let line= str.split(' ')
    let arr=[]
    
    for(let i=0;i<line.length;i++){
        arr.push(line[i].length)
    }
    let max=Math.max(...arr)
    for(let i=0;i<line.length;i++){
        if(line[i].length==max){
            return line[i]
        }
    }
}
console.log(CheckString(str))
```

##  27. Output of this?
```javascript
var Y = 1;
if (function F(){})
{
Y += typeof F;

}
console.log(Y);
```

## 28. Output of this?
```javascript
(()=>{
    var a = b = 3;
})();
console.log("a defined? " + (typeof a !== undefined));
console.log("b defined? " + (typeof b !== undefined));
```
## 29. Write a code to find the unique word from the string?
 
     INPUT:"HELLO HELLO BYE BYE HI"
     OUTPUT:HI
 
 ```javascript
 let unique=(str)=>{
    let arr=[]
    for (let i=0; i<str.length; i++){
        if(str.indexOf(str[i])===str.lastIndexOf(str[i])){
            arr.push(str[i])
        }
    }
    return arr

}
console.log(...unique(str.split(' ')))
```
