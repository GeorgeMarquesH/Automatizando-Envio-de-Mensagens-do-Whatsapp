Automatizando-Envio-de-Mensagens-do-Whatsapp

Este é um mini projeto simples onde criei um script em Python para enviar mensagens personalizadas e anexos automaticamente pelo WhatsApp Web a partir de uma lista no Excel.

Arquivos do Projeto:

automacao_whatsapp.ipynb 
Envios.xlsx 
arquivos

Ferramentas Utilizadas:

Python
Pandas: Para abrir a planilha do Excel e ler os dados das pessoas.
Selenium: Para controlar o navegador (Google Chrome) e fazer os cliques e envios automaticamente.
Urllib: Para formatar o texto da mensagem no formato de link da internet.
OS: Para encontrar o caminho exato dos arquivos no computador.

⚙️ O que o Código Faz:

1. Abertura do Navegador

O Python abre o Chrome e entra no site do WhatsApp Web.
O código espera a tela carregar para dar tempo de conectar via QR Code.

2. Leitura dos Dados

O Pandas lê a planilha Envios.xlsx com os números e mensagens que foram cadastrados.

3. Envio da Mensagem em Loop

Para cada linha da tabela, o script troca o texto "fulano" pelo nome real da pessoa.
O código abre a conversa do número diretamente pelo link do WhatsApp Web.
O sistema verifica se o número existe e clica no botão de enviar a mensagem de texto.

4. Envio de Anexos (Arquivos)

Se houver algum arquivo indicado na planilha (diferente de "N"), o script busca esse arquivo dentro da pasta /arquivos.

Ele clica no clipe de anexo do WhatsApp, insere o arquivo e faz o envio.
