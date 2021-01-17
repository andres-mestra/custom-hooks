# useFetch Hooks

Ejemplo:
```js
const url = 'https://reqres.in/api/users?page=2';

const { data: null, loading: true, error: null } = useFetch(url); 
```