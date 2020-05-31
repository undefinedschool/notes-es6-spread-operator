# ![ES6: Spread operator](https://i.imgur.com/r2wZ2FS.png)


<div align="center">  
  <p align="center">
  <sub>Hola! Soy Nico (<strong>nhsz</strong>), <strong>Dev Full Stack JavaScript y mentor</strong>.</sub>
  </p>
  
  <p align="center">
    <sub>
      Hace un tiempo (principios de 2019) empecé un proyecto llamado <a href="https://undefinedschool.io"><strong>undefined school</strong></a>, una <strong>escuela de Desarrollo Web Full Stack JavaScript</strong>, 100% Open Source, con mentorías personalizadas para grupos reducidos y el foco puesto en los <strong>fundamentos</strong> y <strong>conceptos avanzados</strong>.
    </sub>
  </p>

  <p align="center">
    <sub>
      Me interesa mucho la intersección entre la educación y la tecnología, por eso también participo en proyectos como <a href="https://freecodecampba.org">freeCodeCampBA</a> (co-founder y co-organizador) y <a href="https://twitter.com/LXBA_">Learning Experience BA</a> (co-founder y co-organizador).
    </sub>
  </p>

 <p align="center">
    <sub>
  👉 Si estás arrancando en el mundo del desarrollo web y necesitás una mano, podés encontrarme en <a href="https://twitter.com/_nhsz/">Twitter</a> (también para hablar sobre cualquier tema relacionado a JavaScript o <em>#nerdeadas</em> en general 😛).
  </sub>
  </p>
  
  <p align="center">
  <sub>
    Por último, te cuento que soy muy fan del café (obvio que negro y sin azúcar), asi que si las notas te resultaron útiles y querés colaborar para que no me quede dormido y siga escribiendo guías, apuntes y más <strong>contenido Open Source en español</strong>, podés invitarme uno, gracias! ❤️
  </sub>
  </p>
  
  <p align="center">
  ☕
  <code> 
  <a href="https://cafecito.app/nhsz">
    <strong>Invitame 1 café!</strong>
  </a>
  </code>
  </p>
  <hr>
</div>

👉 Ver [todas las notas](https://github.com/undefinedschool/notes)

---

El _spread operator_ se utiliza para _dispersar_ los elementos de una _colección_ (objeto con ciertas propiedades) iterable (por ejemplo [`Array`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array), [`Map`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Map) y [`Set`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Set)), y tratarlos como cosas sueltas

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
