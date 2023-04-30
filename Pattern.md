# Pattern Based Question
Q1.
```
*
* *
* * *
* * * *
* * * * *
```
```javascript
let triangle=(n)=>{
    for(let i=1;i<=n;i++){
        let str=''
        for (let j=1;j<=i;j++) {
            str+='*'
        }
        console.log(str)
    }
}
triangle(5)
```

Q2.
```
* * * * *
* * * *
* * *
* *
*
```
```javascript
let triangle=(n)=>{
    for(let i=1;i<=n;i++){
        let str=''
        for (let j=i;j<=n;j++) {
            str+='*'
        }
        console.log(str)
    }
}
triangle(5)
```

Q3.
```
     * 
    * *
   * * *
  * * * *
 * * * * *
```
```javascript
let triangle=(n)=>{
    for(let i=1;i<=n;i++){
        let str=''
        for(let j=i;j<=n;j++) {
            str+=' '
        }
        for (let k=1; k<=i; k++) {
            str+='* '
        }
        console.log(str)
    }
}
triangle(5)
```

Q4.
```
          * 
        * *
      * * *
    * * * *
  * * * * *
```
```javascript
let triangle=(n)=>{
    for(let i=1;i<=n;i++){
        let str=''
        for(let j=i;j<=n;j++) {
            str+='  '
        }
        for (let k=1; k<=i; k++) {
            str+='* '
        }
        console.log(str)
    }
}
triangle(5)
```

Q5.
```
  * * * * *
   * * * *
    * * *
     * *
      *
```
```javascript
let triangle=(n)=>{
    for(let i=1;i<=n;i++){
        let str=''
        for (let k=1; k<=i; k++) {
            str+=' '
        }
        for(let j=i;j<=n;j++) {
            str+=' *'
        }
        console.log(str)
    }
}
triangle(5)
```

Q6.
```
   * * * * *
     * * * *
       * * *
         * *
           *
```
```javascript
let triangle=(n)=>{
    for(let i=1;i<=n;i++){
        let str=''
        for (let k=1; k<=i; k++) {
            str+='  '
        }
        for(let j=i;j<=n;j++) {
            str+=' *'
        }
        console.log(str)
    }
}
triangle(5)
```

Q7.
```
1
1 2
1 2 3
1 2 3 4
1 2 3 4 5
```
```javascript
let triangle=(n)=>{
    for(let i=1;i<=n;i++){
        let no=''
        for (let k=1; k<=i; k++) {
            no+=k
        }
        console.log(no)
    }
}
triangle(5)
```

Q8.
```
1
2 2
3 3 3
4 4 4 4
5 5 5 5 5
```
```javascript
let triangle=(n)=>{
    for(let i=1;i<=n;i++){
        let no=''
        for (let k=1; k<=i; k++) {
            no+=i
        }
        console.log(no)
    }
}
triangle(5)
```

Q9.
```
1 
2 3
4 5 6
7 8 9 10
11 12 13 14 15
```
```javascript
let triangle=(n)=>{
    let count =1
    for(let i=1;i<=n;i++){
        let no=''
        for (let k=1; k<=i; k++) {
            no+=count+' '
            count++
        }
        console.log(no)
    }
}
triangle(5)
```

Q10.
```
000000000
?0000000?
??00000??
???000???
????0????
```
```javascript
 let triangle=(n)=>{
    let count =1
    for(let i=1;i<=n;i++){
        let no=''
        for (let k=1; k<i; k++) {
            no+='?'
        }
        for(let j=i;j<=n;j++){
            no+='0'
        }
        for(let j=i;j<n;j++){
            no+='0'
        }
        for (let k=1; k<i; k++) {
            no+='?'
        }
        console.log(no)
        }
}
triangle(5)
```

Q11.
```
<!-- Odd Even -->
1 
0 0
1 1 1
0 0 0 0
1 1 1 1 1
```
```javascript
let triangle=(n)=>{
    for(let i=1;i<=n;i++){
        let no=''
        for (let k=1; k<=i; k++) {
            if(i%2==0){
                no+=0+' '
            }else{
                no+=1+' '
            }
        }
        console.log(no)
    }
}
triangle(5)
```

Q12.
```
<!-- Odd Even -->
0 
1 0
1 0 1
0 1 0 1
0 1 0 1 0
```
```javascript
 let triangle=(n)=>{
    let count =1
    for(let i=1;i<=n;i++){
        let no=''
        for (let k=1; k<=i; k++) {
            if(count%2==1){
                no+=0+' '
            }else{
                no+=1+' '
            }
            count++
        }
        console.log(no)
    }
}
triangle(5)
```

Q13.
```
<!-- Odd Even -->
0 
0 1
0 1 0 
0 1 0 1
0 1 0 1 0
```
```javascript
let triangle=(n)=>{
    for(let i=1;i<=n;i++){
        let no=''
        for (let k=1; k<=i; k++) {
            if(k%2==0){
                no+=1+' '
            }else{
                no+=0+' '
            }
        }
        console.log(no)
    }
}
triangle(5)
```

