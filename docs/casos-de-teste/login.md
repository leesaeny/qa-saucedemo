# Casos de teste | Login

**Aplicação:** SauceDemo
**Tipo:** Funcional manual

## SD-CT-09 | Usuário incorreto

**Pré-condição:** Estar na tela de login.

**Dados de teste:**
- Usuário: `standard_use`
- Senha: `secret_sauce`

**Passos:**
1. Preencher o usuário.
2. Preencher a senha.
3. Clicar em Login.

**Resultado esperado:** A autenticação deve ser recusada, com apresentação de uma mensagem de erro.

## SD-CT-10 | Senha incorreta

**Pré-condição:** Estar na tela de login.

**Dados de teste:**
- Usuário: `standard_user`
- Senha: `secret_sauc`

**Passos:**
1. Preencher o usuário.
2. Preencher a senha.
3. Clicar em Login.

**Resultado esperado:** A autenticação deve ser recusada, com apresentação de uma mensagem de erro.

## SD-CT-11 | Credenciais válidas

**Pré-condição:** Estar na tela de login.

**Dados de teste:**
- Usuário: `standard_user`
- Senha: `secret_sauce`

**Passos:**
1. Preencher o usuário.
2. Preencher a senha.
3. Clicar em Login.

**Resultado esperado:** O usuário deve ser autenticado e direcionado ao catálogo de produtos.
