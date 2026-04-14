# Authentication Test Cases

## Cobertura

Fluxos de login, validacao basica e encerramento de sessao.

| ID | Titulo | Prioridade | Pre-condicoes | Passos principais | Resultado esperado |
| --- | --- | --- | --- | --- | --- |
| TC-AUTH-001 | Login com credenciais validas | Alta | Usuario valido disponivel | Acessar login, informar credenciais validas, enviar formulario | Usuario entra com sucesso e sessao fica autenticada |
| TC-AUTH-002 | Login com senha invalida | Alta | Usuario valido conhecido | Acessar login, informar usuario valido e senha invalida, enviar | Sistema bloqueia acesso e exibe mensagem adequada |
| TC-AUTH-003 | Login com campos obrigatorios vazios | Alta | Nenhuma | Abrir login, deixar campos obrigatorios vazios, tentar enviar | Campos obrigatorios sao destacados ou validados sem autenticar |
| TC-AUTH-004 | Logout apos login bem-sucedido | Alta | Usuario autenticado | Acionar logout | Sessao e encerrada e usuario nao permanece autenticado |
| TC-AUTH-005 | Navegacao para area autenticada sem sessao valida | Media | Usuario deslogado | Tentar acessar area restrita ou acao que exija login | Sistema solicita autenticacao ou redireciona corretamente |

## Observacoes

- registrar a mensagem apresentada em fluxos negativos
- observar comportamento de sessao apos refresh ou navegacao entre paginas principais
