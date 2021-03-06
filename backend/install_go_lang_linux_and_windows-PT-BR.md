
## Como instalar o **Go Lang** em máquinas *Linux* e *Windows* :

Go é uma linguagem de programação que nasceu da frustração no Google. Os desenvolvedores precisavam escolher continuamente uma linguagem que fosse executada com eficiência, mas demoravam muito tempo para compilar ou escolher uma linguagem fácil de programar, mas que era executada de forma ineficiente em produção. O Go foi projetado para ter todas as três características disponíveis ao mesmo tempo: compilação rápida, facilidade de programação e execução eficiente em produção.

### Instalando no Linux Ubuntu 18.04:

```bash sudo apt-get update ```

```bash sudo apt-get upgrade ```

Antes de baixar o Go, certifique-se de estar no diretório home (~):


``` cd ~ ```

Quando o terminal estiver aberto, você instalará manualmente os binários do Go. Embora você possa usar um gerenciador de pacotes, percorrer as etapas de instalação manual o ajudará a entender as alterações de configuração necessárias ao sistema para ter um workspace Go válido.

Use o *curl* para recuperar a URL do tarball que você copiou da página oficial de downloads do Go:

``` curl -O https://dl.google.com/go/go1.12.1.linux-amd64.tar.gz  ```


Em seguida:

``` sha256sum go1.12.1.linux-amd64.tar.gz ```

O hash que é exibido a partir da execução do comando acima deve corresponder ao hash que estava na página de downloads. Se não, então este não é um arquivo válido e você deve baixar o arquivo novamente.

``` 
Output
2a3fdabf665496a0db5f41ec6af7a9b15a49fbe71a85a50ca38b1f13a103aeec  go1.12.1.linux-amd64.tar.gz 
``` 

Em seguida, extraia o arquivo baixado e instale-o no local desejado no sistema. É considerado uma boa prática mantê-lo em /usr/local:

``` sudo tar -xvf go1.12.1.linux-amd64.tar.gz -C /usr/local ``` 

Você terá agora um diretório chamado go no diretório /usr/local. Em seguida, altere recursivamente o proprietário e o grupo deste diretório para root:


``` sudo chown -R root:root /usr/local/go ```

Isso protegerá todos os arquivos e garantirá que apenas o usuário root possa executar os binários do Go.

Nesta etapa, você baixou e instalou o Go na sua máquina Ubuntu 18.04. Na próxima etapa, você configurará seu workspace de **Go**.

Testando se o Go esta instalado usando o comando para verificar a versão.

 
``` go version ```

### Windows 10

Para instalar o Go basta deslocar-nos ao site da linguagem e clicar no botão azul que diz “Download Go” por baixo da mascote, o gopher, que é uma espécie de roedor. Ao clicar somos encaminhados para uma página que contém todas as opções de download para os diversos sistemas operativos.


https://golang.org/

Pré-requisitos
Você precisará de uma máquina com Windows 10 - com acesso administrativo e conectada à Internet.

Passo 1 — Abrindo e configurando o PowerShell

Passo 2 — Instalando o gerenciador de pacotes Chocolatey


## Agora no menu iniciar do Windows escrevemos **variáveis de ambiente**, no meu caso em inglês mas deve ser algo semelhante à seguinte:


Referência:

https://www.digitalocean.com/community/tutorials/como-instalar-o-go-e-configurar-um-ambiente-de-programacao-local-no-ubuntu-18-04-pt



Oficial Go Lang Web Site:

https://golang.org/