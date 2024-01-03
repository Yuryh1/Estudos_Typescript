```typescript

// Em TypeScript, um type é um tipo de objeto que pode ser usado para definir a forma de um objeto. Ele pode ser usado para especificar o nome e o tipo de cada propriedade do objeto.

  

type User = {

    fisrtName: string;

    age:number;

    email:string;

    password:string;

    orders:string[]

};

  

const user:User = {

  fisrtName: "fallen",

  age: 31,

   email:"asdasdaq@gmail.com",

   password:"12321312321",

   orders:["1", "2"]

  
  

}

  

type User2 = {

    fisrtName2: string;

    age2:number;

    email2?:string; // ? torna opcional o uso

    password2?:string; // ? torna opcional o uso

}

  

const user2:User2 = {

  fisrtName2: "fallen",

  age2: 31,

  
  

}

  

//unions

type Author = {

    books:string[]

}

  

const author : Author & User = {

    age: 31,

    books: ['2'],

    email:"asdasdasdasda",

    fisrtName:"asdadasdasda",

    orders:[],

    password:"asdasdasda"

  

}