# Midas: atualizações

Este repositório guarda só os **pacotes de atualização** do Midas, o programa financeiro e de notas fiscais da
associação. Ele é público para que o Midas instalado em cada computador consiga baixar as versões novas sem login.
Não há código-fonte nem dados aqui: o código fica no repositório privado do projeto; notas, planilhas e o banco de
dados ficam só no computador de quem usa.

Este arquivo é gerado a cada publicação a partir do [NOVIDADES.md](NOVIDADES.md), que é o mesmo texto que o Midas
mostra em Ajustes → Atualizações e novidades.

## Versões

| Versão | Data | O que mudou | Pacote |
|---|---|---|---|
| **1.6.0** | 06/10/2026 | Categorias de despesa e de receita, com subcategorias (ex.: Alimentação › Coffee break). Já vêm categorias de receita: Patrocínios, Inscrições, Mensalidades, Doações e Outras receitas. Filtrar por uma categoria mostra também as subcategorias dela.<br>Nova seção Fornecedores: fornecedores e clientes com quanto foi pago e recebido de cada um e a data do último lançamento. Clique num nome para ver todo o histórico dele em Lançamentos.<br>Os fornecedores são cadastrados sozinhos pelo CNPJ das notas arquivadas (inclusive as que você já tinha); num lançamento sem nota, é só digitar o nome do fornecedor ou cliente.<br>Painel do mês com despesas, receitas e saldo. A planilha ganhou a aba Receitas e o bloco "Resultado do mês" (receitas, despesas e saldo); a aba das notas agora se chama Despesas.<br>Lançamentos: novo período "Tudo", para ver todos os meses de uma vez. | [zip, 284 KB](aplicativo/midas-app-1.6.0.zip) |
| **1.5.1** | 06/10/2026 | Correção: a planilha do mês não abria quando havia uma despesa sem nota no mesmo dia de uma nota.<br>Na planilha, despesas sem nota aparecem como "(sem nota)" e mostram o comprovante, se houver.<br>Histórico completo de versões em Ajustes → Atualizações e novidades, com a versão instalada marcada e o que está planejado ("Em breve"). O mesmo histórico fica no GitHub. | [zip, 277 KB](aplicativo/midas-app-1.5.1.zip) |
| **1.5.0** | 06/10/2026 | Receitas e despesas sem nota: botão "Novo lançamento" na seção Lançamentos (patrocínio, inscrições, mensalidades, aluguel...), com comprovante opcional.<br>Contas (caixa, banco e cartão) com saldo, em Ajustes → Contas. Os saldos aparecem no topo dos Lançamentos; clique numa conta para ver só os lançamentos dela.<br>Situação de cada lançamento: pago ou a pagar, recebido ou a receber, previsto, com vencimento. Cancelar não apaga: o lançamento sai das contas e pode ser reativado.<br>Forma de pagamento lida do XML e do cupom (PIX, cartão, dinheiro, boleto...). Na ficha da nota dá para escolher a conta e a forma antes de arquivar.<br>Clique num lançamento para ver e editar; o de uma nota abre com o botão "Abrir a nota". | [zip, 276 KB](aplicativo/midas-app-1.5.0.zip) |
| **1.4.0** | 06/10/2026 | Nova seção Lançamentos (no topo, ao lado de Notas): tudo o que entrou e saiu no mês ou no ano, com busca, filtros por tipo, categoria, grupo e situação, e despesas, receitas e saldo no rodapé.<br>Cada nota arquivada vira um lançamento de despesa; as notas que você já arquivou foram convertidas (com cópia de segurança antes).<br>Painel do mês, gasto dos grupos e planilha agora saem dos lançamentos: os números sempre batem entre si. | [zip, 264 KB](aplicativo/midas-app-1.4.0.zip) |
| **1.3.2** | 06/10/2026 | Leitura de fotos mais rápida: cupons como pedidos de atacado agora são lidos numa passada só, e a foto do celular é reduzida antes da leitura (cerca de 35% menos tempo).<br>Enquanto lê, a lista de envios mostra os segundos ("Lendo… 4 s").<br>O log (dados\log.txt) registra quanto tempo cada etapa da leitura levou, para acharmos o que ainda demora. | [zip, 256 KB](aplicativo/midas-app-1.3.2.zip) |
| **1.3.1** | 06/10/2026 | Primeira foto mais rápida: o leitor de fotos já fica pronto enquanto o Midas abre.<br>Fotos bem lidas na primeira passada não passam pela segunda (até 40% mais rápido nelas).<br>Envio em lote mais leve: cada nota que chega entra na lista sem recarregar tudo.<br>O Midas abre mais rápido quando a leitura pelo Claude está configurada. | [zip, 255 KB](aplicativo/midas-app-1.3.1.zip) |
| **1.3.0** | 06/10/2026 | Atualizações automáticas: o Midas avisa quando há versão nova e baixa só o que mudou (cerca de 250 KB, em vez dos 64 MB do instalador).<br>Se uma versão nova não abrir, o Midas volta sozinho para a anterior.<br>Cópia de segurança do banco todo dia e antes de cada mudança na estrutura; Restaurar_backup.bat para voltar uma cópia. | [zip, 254 KB](aplicativo/midas-app-1.3.0.zip) |
| **1.2.0** | 06/10/2026 | Nova interface: topo enxuto, ficha com fornecedor e valor em destaque, categorias em botões.<br>Nota de XML desenhada como papel e destaques na foto de onde cada campo foi lido.<br>Painel do mês quando não há nada para conferir. | no instalador |
| **1.1.0** | 06/10/2026 | Leitor de fotos no próprio computador, sem internet e sem conta de IA.<br>Instalador único com tudo dentro. | no instalador |
| **1.0.0** | — | Leitura de nota fiscal por XML, PDF e foto, com o documento ao lado dos campos para conferir.<br>Grupos e categorias editáveis; o arquivo vai para a pasta do grupo e a nota entra na planilha mensal do Excel.<br>Envio em lote, modo escuro e aviso quando o documento é um pedido ou comprovante, não uma nota fiscal.<br>Programa Midas.exe, que abre numa janela própria. | no instalador |

## Próximas versões (planejado)

- Contas a pagar e a receber: vencimentos da semana e atrasados, lançamentos recorrentes (aluguel, internet, contador), leitura de boleto, importação do extrato do banco e conciliação.
- Visão financeira: fluxo de caixa previsto e realizado, resultado do mês, alertas de orçamento, painel anual e prestação de contas por evento.

## Como funciona

- `versoes.json`: a versão mais recente do aplicativo, com tamanho e SHA-256 do pacote; o Midas consulta este arquivo.
- `aplicativo/midas-app-<versão>.zip`: o código do Midas de cada versão (cerca de 300 KB). Nenhum pacote é apagado
  nem alterado depois de publicado.
- O instalador completo (Python e leitor de fotos, cerca de 64 MB) só muda quando o motor muda; o link fica em
  `versoes.json`.
- O Midas confere tamanho e SHA-256, troca o aplicativo ao abrir de novo e volta sozinho para a versão anterior se a
  nova não abrir.
