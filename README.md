# Proj-modelagem-de-software
## Projeto 1 - Diagrama de Casos de Uso ##

<img width="4884" height="3796" alt="image" src="https://github.com/user-attachments/assets/0bc6c3fa-d8e8-44ac-9558-59c7e0037273" />



| Identificação | Descrição breve | Ator | Fluxo (resumo) |
|---|---|---|---|
| UC001 — Manter Sessões e Salas | Cadastra e atualiza salas e sessões do cinema. | Administrador | Acessa admin → cria/edita sala/sessão → valida conflitos → salva/publica. |
| UC002 — Manter Filmes | Cadastra, edita ou inativa filmes do catálogo. | Administrador | Abre catálogo → cria/edita filme → valida campos → salva/disponibiliza. |
| UC003 — Importar Títulos da ANCINE | Importa a lista oficial de títulos e atualiza o catálogo local. | Administrador | Solicita importação → sistema consulta ANCINE → valida dados → atualiza catálogo → registra resultado. |
| UC004 — Gerar Relatórios Gerenciais | Consolida dados de vendas/reservas (renda, ingressos, meia-entrada) e gera relatório por critérios (sessão, filme, período). | Administrador | Seleciona filtros → sistema busca dados de vendas/reservas → calcula ingressos e renda por sessão → consolida meia-entrada por categoria → gera relatório. |
| UC005 — Consultar Histórico de Vendas | Consulta vendas registradas por filtros e detalhes. | Administrador | Informa filtros → sistema lista vendas → abre detalhe → exibe valores/assentos/status. |
| UC006 — Gerar Relatório Automático Pós-Sessão | Ao final da sessão, consolida automaticamente vendas/reservas e gera o relatório da sessão. | Sistema (Timer) | Detecta fim da sessão → busca vendas/reservas → calcula ingressos/renda → consolida meia-entrada → salva relatório. |
| UC007 — Enviar Relatórios Obrigatórios à ANCINE | Recebe o relatório consolidado do sistema e registra o recebimento (status/protocolo). | ANCINE | Sistema prepara envio → ANCINE recebe dados/arquivo → ANCINE retorna status/protocolo → sistema registra retorno. |
| UC008 — Consultar Filmes e Sessões | Exibe filmes em cartaz e sessões disponíveis. | Cliente / Cliente Fidelidade | Pesquisa filme → lista sessões/horários → seleciona sessão → direciona para reserva. |
| UC009 — Realizar Reserva de Ingressos | Realiza reserva/compra de ingressos para uma sessão. | Cliente / Cliente Fidelidade | Seleciona sessão/qtd → verifica assentos → escolhe assentos → (opcional) meia/fidelidade → confirma. |
| UC010 — Verificar Disponibilidade de Assento | Mostra assentos livres/ocupados da sessão selecionada. | Cliente / Sistema | Carrega mapa → consulta ocupação → marca disponíveis/ocupados → exibe para seleção. |
| UC011 — Emitir Ingresso (Digital/Impresso) | Gera o ingresso após confirmação da compra/reserva. | Cliente / Sistema | Gera identificador/QR → monta ingresso → disponibiliza digital/impresso → registra emissão. |
| UC012 — Validar Meia-Entrada | Valida elegibilidade e aplica desconto de meia-entrada. | Cliente | Seleciona meia → informa categoria → sistema valida → aplica desconto → atualiza total. |
| UC013 — Aplicar Benefício Fidelidade | Aplica benefícios do programa de fidelidade na compra/reserva. | Cliente Fidelidade | Identifica cliente → valida regras → calcula benefício → aplica → registra e atualiza total. |
