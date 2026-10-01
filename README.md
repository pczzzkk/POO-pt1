# Atividade 1

***TypeScript***
```typescript
class Pessoa {
    nome: string;
    idade: number;
}

const pessoa = new Pessoa();

pessoa.nome = "João";
pessoa.idade = 20;

console.log("Nome:", pessoa.nome);
console.log("Idade:", pessoa.idade);
```

# Atividade 2

***TypeScript***
```typescript
class Produto {
    nome: string;
    preco: number;
    estoque: number;

    constructor(nome: string, preco: number, estoque: number) {
        this.nome = nome;
        this.preco = preco;
        this.estoque = estoque;
    }
}

const produto1 = new Produto("Notebook", 3500, 10);
const produto2 = new Produto("Mouse", 80, 25);

console.log("Produto 1:");
console.log("Nome:", produto1.nome);
console.log("Preço: R$", produto1.preco);
console.log("Estoque:", produto1.estoque);

console.log("\nProduto 2:");
console.log("Nome:", produto2.nome);
console.log("Preço: R$", produto2.preco);
console.log("Estoque:", produto2.estoque);
```

# Atividade 3

***TypeScript***
```typescript
class Aluno {
    nome: string;
    nota: number;

    constructor(nome: string, nota: number) {
        this.nome = nome;
        this.nota = nota;
    }

    aprovado(): boolean {
        return this.nota >= 6;
    }
}

const aluno = new Aluno("Maria", 7.5);

console.log("Nome:", aluno.nome);
console.log("Nota:", aluno.nota);
console.log("Aprovado:", aluno.aprovado());
```
# Atividade 4

***TypeScript***
```typescript
class Retangulo {
    largura: number;
    altura: number;

    constructor(largura: number, altura: number) {
        this.largura = largura;
        this.altura = altura;
    }

    calcularPerimetro(): number {
        return 2 * (this.largura + this.altura);
    }
}

const retangulo = new Retangulo(5, 3);

console.log("Largura:", retangulo.largura);
console.log("Altura:", retangulo.altura);
console.log("Perímetro:", retangulo.calcularPerimetro());
```
# Atividade 5

***TypeScript***
```typescript
```typescript
class ContaBancaria {
    private saldo: number;

    constructor(saldoInicial: number) {
        this.saldo = saldoInicial;
    }

    depositar(valor: number): void {
        if (valor > 0) {
            this.saldo += valor;
        }
    }

    consultarSaldo(): number {
        return this.saldo;
    }
}

const conta = new ContaBancaria(1000);

conta.depositar(500);

console.log("Saldo:", conta.consultarSaldo());
```
