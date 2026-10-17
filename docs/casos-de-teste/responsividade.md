# Casos de teste | Responsividade

**Aplicação:** SauceDemo
**Tipo:** Teste manual de interface e responsividade

## SD-CT-16 | Legibilidade da mensagem de erro no login

**Origem:** Caso identificado durante a exploração do SD-CT-09.

**Pré-condição:** Estar na tela de login do SauceDemo.

**Dados de teste:**
- Usuário: `standard_use`
- Senha: `secret_sauce`
- Navegadores: Chrome, Edge, Safari e Vivaldi

**Passos:**
1. Abrir a aplicação em uma janela larga.
2. Preencher as credenciais inválidas.
3. Clicar em Login.
4. Verificar a legibilidade da mensagem de erro.
5. Reduzir gradualmente a largura da janela.
6. Comparar a apresentação da mensagem.
7. Repetir o procedimento nos quatro navegadores.

**Resultado esperado:** A mensagem deve permanecer integralmente legível, sem cortes ou sobreposição de elementos, nas larguras de janela suportadas.

**Observação:** A largura exata da viewport não foi medida. O teste investiga o comportamento visual, não sua causa técnica.
