# Midas: atualizações

Este repositório guarda só os **pacotes de atualização** do Midas, o programa de notas fiscais da associação. Ele é
público para que o Midas instalado em cada computador consiga baixar as versões novas sem login.

Não há código-fonte nem dados aqui. O código fica no repositório privado do projeto; notas, planilhas e o banco de
dados ficam só no computador de quem usa.

Estrutura prevista (em construção):

- `versoes.json`: a versão mais recente do aplicativo e do motor, com o tamanho e o SHA-256 de cada pacote
- `aplicativo/`: pacotes do código do Midas (cerca de 1 MB cada), um por versão
- `motor/`: pacotes do Python e do leitor de fotos, publicados só quando mudam
- `NOVIDADES.md`: o que mudou em cada versão
