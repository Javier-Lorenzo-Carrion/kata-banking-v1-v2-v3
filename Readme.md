# Template TypeScript
## Diseño Sostenible - Ingeniería y Artesanía del Software con TypeScript
![Diseño Sostenible](coverds.png)

Plantilla base para practicar las katas del curso o para empezar un proyecto nuevo.

Incluye:
* TypeScript
* Jest
* ESLint
* Prettier
* Husky

## Instrucciones
* `nvm use`
* `npm install`
* `npm test`

Más información sobre el curso en [diseñosostenible.com](https://diseñosostenible.com).

### ESLint
[TypeScript ESLint Rules](https://github.com/typescript-eslint/typescript-eslint/tree/master/packages/eslint-plugin)

### Husky hooks
* Pre-commit: Execute npm analize (tsc + eslint --fix)
* Pre-push: Execute test

## Requisitos de la kata

Tu banco de toda la vida está cansado de su software de contabilidad hecho en Cobol y te ha contratado para que empieces desde cero tu greenfield project y, además, te deja hacerlo con nuestra tecnología favorita, así que adelante con TypeScript.

* La aplicación debe hacer un depósito en la cuenta
* La aplicación debe permitir hacer una retirada de la cuenta
* La aplicación debe imprimir los asientos de la cuenta a través de la consola con el siguiente formato de ejemplo:

Date | Amount | Balance

14/01/2025 | 20 | 20

15/01/2025 | 10 | 30

16/01/2025 | -5 | 25

Se debe respetar la interfaz de la clase y no se puede añadir ningún otro método público. La interfaz en cuestión es:

```
export class Account {
    deposit(amount: number): void
    withdraw(amount: number): void
    printStatement(): void
}

```
