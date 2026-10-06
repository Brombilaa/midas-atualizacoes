# Novidades do Midas

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
