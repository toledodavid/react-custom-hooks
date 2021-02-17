# Custom Hooks

## useCounter
Para crear un contador y usarlo en un componente.

Ejemplo de uso:
```js
const {counter, increment, decrement, reset} = useCounter(5);
```

## useFetch
Para hacer peticiones a un endpoint de una API y mostrar la siguiente informacion en el componente que se esta usando (data, loading, error).

Ejemplo de uso:
```js
const {loading, data, error} = useFetch(`https://www.breakingbadapi.com/api/quotes/1`);
```

## useForm
Para manejar los datos de los inputs en formularios que usamos en un componente.

Ejemplo de uso:
```js
const [formValues, handleInputChange] = useForm({
  name: '',
  email: '',
  password: ''
});

const {name, email, password} = formValues;
```
