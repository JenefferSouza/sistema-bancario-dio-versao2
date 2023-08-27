# DESAFIO - Otimizando o sistema bancário com funções Python (DIO)

Precisamos deixar nosso código mais modularizado, para isso vamos criar funções para as operações existentes da [versão 1](https://github.com/JenefferSouza/sistema-bancario-dio) do nosso programa: sacar, depositar e visualizar extrato. Além disso, para a versão 2 do sistema precisamos criar duas novas funções: criar usuário (cliente do banco) e criar conta corrente (vincular com usuário).

### Separação em funções
Devemos criar funções para todas as operações do sistema. Cada função vai ter uma regra na passagem de argumentos. O retorno e a forma como serão chamadas pode ser definida por você da forma que achar melhor.

### Saque
A funçãosaque deve receber os argumentos apenas por nome (Keyword Only). Sugestão de argumento: saldo, valor, extrato, limite, numero_saque, limite_saques. Dugestão de retorno: saldo e extrato.

### Depósito
A função depósito deve receber argumentos apenas por posição (Positional Only). Sugestão de argumentos: saldo, valor, extrato. Sugestão de retorno: saldo e extrato.

### Extrato
A função extrato deve receber os argumentos por posição e nome (Positional Only and Keyword Only). Argumentos posicionais: saldo, argumentos nomenais: extrato.

### Novas Funções
Precisamos criar duas novas funções: criar usuário e criar conta corrente. Fique a vontade para adicionar mais funções, exemplo: listar contas.

### Criar usuário (cliente)
O programa deve argumentar os usuários em uma lista, um usuário é composto por: nome, data de nascimento, cpf e endereço. O endereço é uma string com o formato: logradouro, nº - bairro - cidade/sigla do estado. Deve ser armazenado somente os números do CPF (string). Não podemos cadastrar 2 usuários com o mesmo CPF.

### Criar conta corrente
O programa deve armazenar contas em uma lista, uma conta é composta por: agência, número de conta e usuário. O número da conta é sequêncial, iniciando em 1. O número da agência é fixo: "0001". O usuário pode ter mais de uma conta, mas uma conta pertence a somente um usuário.

### Dica
Para vincular um usuário a uma conta, filtre a lista de usuários buscando o número do CPF informado para cada usuário da lista.