# useForm Hook

## Ejemplo de uso(Retorna):


* las variables necesarias para los inputs (declarandolos en el initialForm)

* La funcion cuando nota un cambio en el respectivo input

* La funcion para resetear todos los input
#

Inicializacion del hook
```js
const initialForm = {
    name: '',
    age: 0,
    email: '',
}
const {formValues, handleInputChange, resetInput}= useForm(initalForm);

```

Desestructuracion del formValues
```js
const { name, age, email } = formValues;
```

Creacion del input en html
```Html
<input
    type="text"
    name='name'
    value={name}
    onChange={handleInputChange} />
<input>
```
