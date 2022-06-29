# JAVASCRIPT INTERFACES E HERANCA EM POO

## HERANÇA

```javascript

export class Conta {
  constructor() {
    // logic
  }

  contaMethod() {
    console.log('Print em Conta')
  }
}

// extends = pega tudo que tem em `Conta` para poder utilizar aqui em `ContaCorrente`
export class ContaCorrente extends Conta {
  constructor() {
    // Chama o construtor da classe pai (Conta)
    super(param1, param2, paramN)
  }

  contaCorrenteMethod() {
    super.contaMethod()
    console.log('Print em Conta Corrente')
  }
}

// Será printado primeiro
Print em Conta
// Após
Print em Conta Corrente

// Podendo assim chamar o metodo da classe pai
```

### PUBLIC E PRIVATE

```javascript

// Método publico
method() {
  // logic
}

// Método privado
_method() {
  // logic
}

// Podendo haver a instância entre eles
method() {
  this._method()
}

```

## ABSTRATA

Ela serve apenas para ser herdada e não instanciada.

## POLIFORMISMO

Objetos de classes diferentes sendo tratados da mesma maneira
