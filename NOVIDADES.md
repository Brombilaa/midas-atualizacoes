# Novidades do Midas

O que mudou em cada versão, da mais nova para a mais antiga. A seção "Próximas versões" é o planejado, ainda não
instalado; ela muda conforme o trabalho avança.

## Próximas versões
- 1.8.0: lançamentos recorrentes (aluguel, internet, contador...) cadastrados no Midas, que geram os próximos meses como "previsto"; leitura de boleto pela linha digitável colada e pelo PDF.
- 1.9.0: avisos também fora do Midas, ligados em Ajustes (notificação do Windows pela manhã e resumo por e-mail), e o polimento depois de algumas semanas de uso real.
- Depois: visão financeira (fluxo de caixa previsto e realizado, resultado do mês, alertas de orçamento, painel anual e prestação de contas por evento).

## 1.7.0 · 2026-10-06
- Nova seção Agenda: contas atrasadas, de hoje, dos próximos 7 dias, do resto do mês e mais adiante, com o total a pagar e a receber de cada faixa.
- Pagar ou receber com um clique, direto da Agenda: data, conta e comprovante, sem abrir o lançamento.
- Ao arquivar uma nota, escolha "Já paga" (o padrão) ou "A pagar" com o vencimento; a nota a pagar vai para a Agenda.
- Vários documentos no mesmo lançamento: nota, boleto, comprovante, recibo, pedido. Num lançamento novo, dá para anexar antes de salvar.
- Pedido e nota fiscal da mesma compra: o Midas mostra "Parece a mesma compra" e junta as duas num lançamento só, com os dois arquivos.
- Ao abrir o Midas, um aviso mostra as contas atrasadas e as da semana; o número na aba Agenda fica vermelho quando há atraso.

## 1.6.0 · 2026-10-06
- Categorias de despesa e de receita, com subcategorias (ex.: Alimentação › Coffee break). Já vêm categorias de receita: Patrocínios, Inscrições, Mensalidades, Doações e Outras receitas. Filtrar por uma categoria mostra também as subcategorias dela.
- Nova seção Fornecedores: fornecedores e clientes com quanto foi pago e recebido de cada um e a data do último lançamento. Clique num nome para ver todo o histórico dele em Lançamentos.
- Os fornecedores são cadastrados sozinhos pelo CNPJ das notas arquivadas (inclusive as que você já tinha); num lançamento sem nota, é só digitar o nome do fornecedor ou cliente.
- Painel do mês com despesas, receitas e saldo. A planilha ganhou a aba Receitas e o bloco "Resultado do mês" (receitas, despesas e saldo); a aba das notas agora se chama Despesas.
- Lançamentos: novo período "Tudo", para ver todos os meses de uma vez.

## 1.5.1 · 2026-10-06
- Correção: a planilha do mês não abria quando havia uma despesa sem nota no mesmo dia de uma nota.
- Na planilha, despesas sem nota aparecem como "(sem nota)" e mostram o comprovante, se houver.
- Histórico completo de versões em Ajustes → Atualizações e novidades, com a versão instalada marcada e o que está planejado ("Em breve"). O mesmo histórico fica no GitHub.

## 1.5.0 · 2026-10-06
- Receitas e despesas sem nota: botão "Novo lançamento" na seção Lançamentos (patrocínio, inscrições, mensalidades, aluguel...), com comprovante opcional.
- Contas (caixa, banco e cartão) com saldo, em Ajustes → Contas. Os saldos aparecem no topo dos Lançamentos; clique numa conta para ver só os lançamentos dela.
- Situação de cada lançamento: pago ou a pagar, recebido ou a receber, previsto, com vencimento. Cancelar não apaga: o lançamento sai das contas e pode ser reativado.
- Forma de pagamento lida do XML e do cupom (PIX, cartão, dinheiro, boleto...). Na ficha da nota dá para escolher a conta e a forma antes de arquivar.
- Clique num lançamento para ver e editar; o de uma nota abre com o botão "Abrir a nota".

## 1.4.0 · 2026-10-06
- Nova seção Lançamentos (no topo, ao lado de Notas): tudo o que entrou e saiu no mês ou no ano, com busca, filtros por tipo, categoria, grupo e situação, e despesas, receitas e saldo no rodapé.
- Cada nota arquivada vira um lançamento de despesa; as notas que você já arquivou foram convertidas (com cópia de segurança antes).
- Painel do mês, gasto dos grupos e planilha agora saem dos lançamentos: os números sempre batem entre si.

## 1.3.2 · 2026-10-06
- Leitura de fotos mais rápida: cupons como pedidos de atacado agora são lidos numa passada só, e a foto do celular é reduzida antes da leitura (cerca de 35% menos tempo).
- Enquanto lê, a lista de envios mostra os segundos ("Lendo… 4 s").
- O log (dados\log.txt) registra quanto tempo cada etapa da leitura levou, para acharmos o que ainda demora.

## 1.3.1 · 2026-10-06
- Primeira foto mais rápida: o leitor de fotos já fica pronto enquanto o Midas abre.
- Fotos bem lidas na primeira passada não passam pela segunda (até 40% mais rápido nelas).
- Envio em lote mais leve: cada nota que chega entra na lista sem recarregar tudo.
- O Midas abre mais rápido quando a leitura pelo Claude está configurada.

## 1.3.0 · 2026-10-06
- Atualizações automáticas: o Midas avisa quando há versão nova e baixa só o que mudou (cerca de 250 KB, em vez dos 64 MB do instalador).
- Se uma versão nova não abrir, o Midas volta sozinho para a anterior.
- Cópia de segurança do banco todo dia e antes de cada mudança na estrutura; Restaurar_backup.bat para voltar uma cópia.

## 1.2.0 · 2026-10-06
- Nova interface: topo enxuto, ficha com fornecedor e valor em destaque, categorias em botões.
- Nota de XML desenhada como papel e destaques na foto de onde cada campo foi lido.
- Painel do mês quando não há nada para conferir.

## 1.1.0 · 2026-10-06
- Leitor de fotos no próprio computador, sem internet e sem conta de IA.
- Instalador único com tudo dentro.

## 1.0.0
- Leitura de nota fiscal por XML, PDF e foto, com o documento ao lado dos campos para conferir.
- Grupos e categorias editáveis; o arquivo vai para a pasta do grupo e a nota entra na planilha mensal do Excel.
- Envio em lote, modo escuro e aviso quando o documento é um pedido ou comprovante, não uma nota fiscal.
- Programa Midas.exe, que abre numa janela própria.
