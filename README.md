# Comparação de Métodos AJAX

Este repositório apresenta uma análise comparativa das principais técnicas para requisições assíncronas em JavaScript, com exemplos práticos de implementação.

## Tecnologias Comparadas

- **XMLHttpRequest (XHR)**: API mais antiga, baseada em callbacks. É verbosa e difícil de
manter, mas compatível com todos os navegadores
- **Fetch API**:  Moderna, baseada em Promises. Possui sintaxe mais limpa, mas requer
AbortController para cancelamento e não envia cookies por padrão.
- **Promises**:  Introduzidas no ES6, facilitam o encadeamento de ações assíncronas e
melhoram o tratamento de erros.
- **Async/Await**: Açúcar sintático para Promises, introduzido no ES8. Permite escrever código
assíncrono com aparência síncrona, facilitando a leitura e manutenção.

##   Conclusões e Recomendações

- **Para projetos modernos**, o uso de Fetch com Async/Await é altamente recomendado.
- **Em casos de compatibilidade** com navegadores antigos, pode-se utilizar XMLHttpRequest.
- **Evite usar callbacks aninhados**; prefira Promises ou Async/Await para código mais limpo e sustentável.
- **Para cancelamento ou controle de progresso**, considere o uso de AbortController com Fetch.


##  Principais Diferenças

| Característica       | XHR          | Fetch        | Promises     | Async/Await  |
|----------------------|--------------|--------------|--------------|--------------|
| Sintaxe              | Verbosa      | Limpa        | Encadeável   | Síncrona     |
| Tratamento de erros  | Complexo     | Then/catch   | Then/catch   | Try/catch    |
| Cancelamento         | Nativo       | Com AbortController | -        | Com AbortController |
| Suporte              | Universal    | Moderno      | ES6+         | ES8+         |



##  Como Usar

```bash
git clone https://github.com/Fernandaallima/ajax-compara-o.git
cd ajax-compara-o
