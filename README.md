> El siguiente contenido fue elaborado por [@_nhsz](https://twitter.com/_nhsz) como guía para las clases de [undefined school](https://twitter.com/undefinedSchool)
> Son bienvenidos los _issues_ y _PRs_ para mejorar el contenido, corregir errores, etc. 

> 👉 Si te resultó útil, **se agradece que lo compartas para que le llegue a más gente!**

# ![ES6: Spread operator](https://i.imgur.com/r2wZ2FS.png)

El _spread operator_ se utiliza para _dispersar_ los elementos de una _colección_ (objeto con ciertas propiedades) iterable (por ejemplo _arrays_ y _sets_), y tratarlos como cosas sueltas

```js
const nums1 = [1, 2, 3];
const nums2 = [4, 5, 6];

console.log(...nums1);

// agregar adelante
console.log([...nums1, 4, 5, 6]);
// concatenar
num2.concat(num1);
console.log([4, 5, 6, ...nums1]);
// magia
console.log([1, ...nums2, 2, 3]);
```

```js
// más magia
function sum(x, y, z) {
  return x + y + z;
}

const numbers = [1, 2, 3];
// si queremos invocar a la función sum con los valores del array numbers...
sum(numbers[0], numbers[1], numbers[2]);

// o podemos usar spread!
console.log(sum(...numbers));
```


```js
// duplicar arrays
const x = [1, 2, 3];
const y = [...x];

console.log(y);
console.log([...x, ...y]);
```

```js
// obtener máximo y mínimo
const x = [1, 2, 3];

console.log(Math.max(...x));
console.log(Math.min(...x));
```
