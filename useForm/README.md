# useForm Hook

Ejemplo:

```js
const initialState = {
  name: '',
  age: 0,
  email: '',
}

cosnt [ values, handleInputChange, reset ] = useForm(initialState)
```