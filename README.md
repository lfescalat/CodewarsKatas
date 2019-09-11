####[Problema #1](https://www.codewars.com/kata/58ce8725c835848ad6000007 "Enlace del problema")

```javascript
const potatoes = (p0, w0, p1) => Math.floor(w0*(100-p0)/(100-p1))
```

####[Problema #2](https://www.codewars.com/kata/5a0d38c9697598b67a000041 "Enlace del problema")

```javascript
const eliminateUnsetBits = number => parseInt(number.replace(/0/g,''),2) || 0
```
####[Problema #3](https://www.codewars.com/kata/5a651865fd56cb55760000e0 "Enlace del problema")

```javascript
const arrayLeaders = numbers => numbers.filter((e,i,arr) => e > arr.slice(i +1, arr.length).reduce((c, e) => c + e, 0))
```

####[Problema #4](https://www.codewars.com/kata/57ee99a16c8df7b02d00045f "Enlace del problema")

```javascript
"use strict";

const flattenAndSort = array => {
  let newArray = []
  array.forEach(e => {
    newArray = newArray.concat(e)
  })
  return newArray.sort((a,b)=> a - b)
}
```

####[Problema #5](https://www.codewars.com/kata/5a99a03e4a6b34bb3c000124 "Enlace del problema")

```javascript
const isPrime = num => {
  for(var i = 2; i < num; i++)
    if(num % i == 0) return false
  return num > 1
}

const numPrimorial = n => {
  let conta = 0
	let prime = []
	while (prime.length != n){
		if (isPrime(conta)){
			prime.push(conta)
        }
		conta++
    }
	 return prime.reduce((a,b) => a * b)
}
```

####[Problema #6](https://www.codewars.com/kata/57b06f90e298a7b53d000a86 "Enlace del problema")

```javascript
const queueTime = (customers, n) => {
  let queueArr = Array(n).fill(0)
  
  customers.forEach((e, i) => {
    queueArr[0] += customers[i]
    queueArr.sort((a,b) => a-b)
  })

  return queueArr[queueArr.length-1]
}
```
####[Problema #7](https://www.codewars.com/kata/521c2db8ddc89b9b7a0000c1 "Enlace del problema")

```javascript
const snail = array => {
  let vector = []
  while (array.length) {
    vector.push(...array.shift())
    array.map(row => vector.push(row.pop()))
    array.reverse().map(row => row.reverse())
  }
  return vector
}
```

####[Problema #8	](https://www.codewars.com/kata/582da6ba06e37f9b75000510 "Enlace del problema")

