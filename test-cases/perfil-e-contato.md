# Profile and Contact Test Cases

## Cobertura

Fluxos secundarios com impacto moderado na experiencia e confianca do produto.

| ID | Titulo | Prioridade | Pre-condicoes | Passos principais | Resultado esperado |
| --- | --- | --- | --- | --- | --- |
| TC-PC-001 | Acesso a dados de perfil por usuario autenticado | Media | Usuario autenticado | Navegar ate a area de conta ou perfil | Dados principais da conta ficam acessiveis sem erro |
| TC-PC-002 | Protecao de area de perfil para usuario nao autenticado | Media | Usuario deslogado | Tentar acessar area de perfil | Sistema solicita login ou redireciona corretamente |
| TC-PC-003 | Envio de formulario de contato com campos validos | Media | Aplicacao acessivel | Preencher formulario de contato com dados validos e enviar | Sistema confirma o envio ou apresenta feedback positivo |
| TC-PC-004 | Validacao de campos obrigatorios no contato | Media | Aplicacao acessivel | Deixar campos obrigatorios vazios e tentar enviar | Sistema impede envio e indica campos faltantes |
| TC-PC-005 | Validacao de formato em campo de email no contato | Media | Aplicacao acessivel | Informar email em formato invalido e enviar | Sistema rejeita o valor e orienta a correcao |

## Observacoes

- estes fluxos entram depois dos caminhos criticos, mas ajudam a demonstrar cobertura funcional mais completa
