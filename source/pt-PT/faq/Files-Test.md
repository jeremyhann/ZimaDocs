---
title: Uso do 7º Bay
description:
type: "Docs"
tip: O formato fixo da barra superior não deve ser removido, a descrição é para a descrição do artigo; se não preenchida, será capturada a primeira parte do conteúdo
---
# Instalar e Remover o 7º Bay
## Preparações:
Certifique-se de que o ZimaCube está desligado e desconectado.
Prepare o disco rígido a ser instalado.
## Passos Específicos:
Passo 1: Remova o painel frontal do gabinete.
![](https://manage.icewhale.io/api/static/docs/1722418820491_image.png)
Passo 2: Remova o 6º bay.
![](https://manage.icewhale.io/api/static/docs/1722418858886_image.png)
Passo 3: Gire no sentido anti-horário para desparafusar os parafusos que prendem o sétimo disco.
![](https://manage.icewhale.io/api/static/docs/1722418913222_image.png)
Passo 4: Remova o 7º bay.
![](https://manage.icewhale.io/api/static/docs/1722418964759_image.png)
![](https://manage.icewhale.io/api/static/docs/1722418974044_image.png)
Passo 5: Instale livremente o SSD no 7º bay.
![](https://manage.icewhale.io/api/static/docs/1722419028169_image.png)
Passo 6: Empurre o 7º bay para a posição correta e aperte os parafusos no sentido horário.
![](https://manage.icewhale.io/api/static/docs/1722419069919_image.png)

# Como atualizar o firmware de iluminação do 7º ZimaCube
*Para evitar a falha do esp32 em atualizações OTA (Over-The-Air), um método de atualização com fio é aqui introduzido.*
## Solução de 3 passos
1. Conectar ao WiFi
Conecte-se ao WiFi com um computador
Nome: "ZimaCube"
Senha: "homecloud"
2. Insira a URL
Digite no navegador: 172.16.1.1
3. Faça o upload do firmware
[https://drive.google.com/file/d/1h8LKvZ47gdMmpJzu6CFK3awjGFX5ayRE/view?usp=drive_link](https://drive.google.com/file/d/1h8LKvZ47gdMmpJzu6CFK3awjGFX5ayRE/view?usp=drive_link)

## Plano de backup

**Preparação antes da atualização**
- Computador
- Cabo de dados tipo-c
- Disco 7
- Baixe e descompacte o pacote comprimido
[https://drive.google.com/file/d/15nPalLy-2ieNQ84dT1gchBzLqtEfM--8/view?usp=drive_link](https://drive.google.com/file/d/15nPalLy-2ieNQ84dT1gchBzLqtEfM--8/view?usp=drive_link)

**Iniciar a atualização**
3.1 Use o cabo de dados tipo-c para conectar o computador ao tipo-c no chip do sétimo disco
3.2 Abra o link [espressif.github.io](espressif.github.io) no computador
3.3 Clique em 'Conectar'
![](https://manage.icewhale.io/api/static/docs/1730360675989_image.png)

3.4 Selecione a porta serial para conexão
![](https://manage.icewhale.io/api/static/docs/1730360689217_image.png)

3.5 Clique em 'DIY'
![](https://manage.icewhale.io/api/static/docs/1730360715808_image.png)

3.6 Clique em 'Adicionar Arquivo' duas vezes
![](https://manage.icewhale.io/api/static/docs/1730360989529_image.png)

3.7 Mude o endereço de gravação e selecione o arquivo
*O endereço de gravação específico é mostrado na figura, selecione os três arquivos após descompactação na ordem*
![](https://manage.icewhale.io/api/static/docs/1730360997291_image.png)

3.8 Clique em 'Programar' para iniciar a gravação
![](https://manage.icewhale.io/api/static/docs/1730361017895_image.png)

3.9 A gravação foi concluída, pressione o botão de reset RST e o firmware foi atualizado com sucesso.