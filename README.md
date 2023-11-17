![Static Badge](https://img.shields.io/badge/STATUS-Em_Desenvolvimento-FFC000)
># Sprint 5 - Ansible/IAC 
<div align="center"> <img src="" /> </div>



># Desafio 1 ![Static Badge](https://img.shields.io/badge/STATUS-Em_Desenvolvimento-FFC000)
Instalar uma VM com OL8, instalar o ANSIBLE e criar um YAML de ping para o IP do seu desktop



### 

ENTRA
```
ENTRA
```
<div align="center"> <img src=""/> </div>



># Desafio 2 ![Static Badge](https://img.shields.io/badge/STATUS-Em_Desenvolvimento-FFC000)
Instalar o terraform no seu desktop e criar o deploy de uma instancia EC t2.micro na AWS


### Instalação do Terraform no Windows 11


O primeiro passo é fazer o download do `Terraform` acessando o endereço abaixo pelo navegador e procurar por `Download` no canto superior direito.
```
https://www.terraform.io/
```
<div align="center"> <img src="https://github.com/bmsousa9/CompassUOL-Semana-05/assets/111213549/90786ae0-b80e-421b-8569-96f9c1f24b4b"/> </div>

Em seguida, localizar a `Windows` e a distribuição que melhor se adapta à configuração local. No meu caso, escolhi o binário `386` na versão 1.6.4 .
```
https://releases.hashicorp.com/terraform/1.6.4/terraform_1.6.4_windows_386.zip
```
<div align="center"> <img src="https://github.com/bmsousa9/CompassUOL-Semana-05/assets/111213549/944a5404-a7ef-494d-995e-295c40c65303"/> </div>

Logo ao terminar o download, descompactei e movi o executável para uma pasta `terraform` na raiz do disco.
<div align="center"> <img src="https://github.com/bmsousa9/CompassUOL-Semana-05/assets/111213549/40921b63-612b-4e3f-a1ed-e756d69f44c1"/> </div>

Na barra de pesquisa, digitei `Exibir configurações avançadas do sistema` e cliquei no item correspondente.
<div align="center"> <img src="https://github.com/bmsousa9/CompassUOL-Semana-05/assets/111213549/e76dda4a-27f2-47c7-941d-50f8506a78fc"/> </div>

Logo em seguida, localizei a aba `Avançado` e cliquei no botão no canto inferior direito, `Variáveis de Ambiente`.
<div align="center"> <img src="https://github.com/bmsousa9/CompassUOL-Semana-05/assets/111213549/51ce8b58-c5b2-4bfa-9eab-1e4261a185e0"/> </div>

Cliquei na linha `Path` em seguida no botão `Editar`.
<div align="center"> <img src="https://github.com/bmsousa9/CompassUOL-Semana-05/assets/111213549/faf08b93-88da-49ff-a6e7-2c34bcb73de9"/> </div>

No botão `Novo`, inseri o caminho da pasta criada anteriormente e em seguida em `OK`. Fechei todas as janelas que surgiram até agora.
<div align="center"> <img src="https://github.com/bmsousa9/CompassUOL-Semana-05/assets/111213549/7982897b-52bd-4451-b37b-911263fafc9e"/> </div>

No teclado, inseri `Windows+R` e digitei `Powershell`.
<div align="center"> <img src="https://github.com/bmsousa9/CompassUOL-Semana-05/assets/111213549/c6250bf7-6065-41eb-a7e6-65fb0d2a5152"/> </div>

Como o Powershell aberto, consegui verificar a instalação com sucesso do Terraform com o comando abaixo:
```
terraform --version
```
<div align="center"> <img src="https://github.com/bmsousa9/CompassUOL-Semana-05/assets/111213549/d9995af1-f6c8-424f-9e94-281f50023323"/> </div>


### Instalação do AWS Command Line Inteface no Windows 11


O primeiro passo foi acessar no site da AWS, o download do `AWS CLI`, logo no canto superior direito em `Windows`
```
https://aws.amazon.com/pt/cli/
```
<div align="center"> <img src="https://github.com/bmsousa9/CompassUOL-Semana-05/assets/111213549/9fd8e2b3-fb57-4496-a9a4-93db57fcd34c"/> </div>

Ao fazer o download e executar o `exe`, avancei com a instalação seguindo os passos que apareciam.
<div align="center"> <img src="https://github.com/bmsousa9/CompassUOL-Semana-05/assets/111213549/bda66b68-fbf3-4e84-bf3f-ddf669eff87f"/> </div>
<div align="center"> <img src="https://github.com/bmsousa9/CompassUOL-Semana-05/assets/111213549/4437f793-b954-495e-956f-6add0b3753df"/> </div>


### Criação de uma conta AWS


O primeiro passo é acessar o site da `AWS` através de um navegador e em seguida clicar em `Crie uma conta da AWS`.
```
https://aws.amazon.com/pt/
```
<div align="center"> <img src="https://github.com/bmsousa9/CompassUOL-Semana-05/assets/111213549/345f2c14-f3a0-4566-a507-6e03f7852ee9"/> </div>

Logo em seguida, entrei com meu e-mail comporativo e nomeei a conta conforme o e-mail.
<div align="center"> <img src="https://github.com/bmsousa9/CompassUOL-Semana-05/assets/111213549/c99a9131-bd7f-4fcd-84e0-80f9b6b205d6"/> </div>

A partir daí recebi um e-mail com o código de verificação que foi necessário para continuar com a criação da senha e da conta.
<div align="center"> <img src="https://github.com/bmsousa9/CompassUOL-Semana-05/assets/111213549/25aed3b5-3099-4e3b-8c46-a51743bd3af6"/> </div>

Nos passos seguintes, é necessário a inserção de um cartão de crédito válido, de um número de celular válido e fazer novamente a verificação. Logo e seguida, escolher a melhor conta para o perfil. Nessa caso, escolhi a gratuita.
<div align="center"> <img src="https://github.com/bmsousa9/CompassUOL-Semana-05/assets/111213549/ba15b7c0-abba-4f6a-bd58-d6c8c95f769d"/> </div>

Com esses passos, foi possível ter acesso ao console da AWS.
<div align="center"> <img src="https://github.com/bmsousa9/CompassUOL-Semana-05/assets/111213549/fe6ae9ff-4d93-43bc-b584-4514933d1011"/> </div>


### Criação de um usuário no AWS Identity and Access Management


No console da AWS, digitei `ami` na caixa de pesquisa e selecionei o serviço correspondente.
<div align="center"> <img src="https://github.com/bmsousa9/CompassUOL-Semana-05/assets/111213549/268a878c-5f31-4f55-b2de-cefa4e9d72bc"/> </div>

No lado esquerdo, localizei `Usuários`.
<div align="center"> <img src="https://github.com/bmsousa9/CompassUOL-Semana-05/assets/111213549/a4b7ecd1-82e8-461a-8cab-fe57ff78091e"/> </div>

O passo seguinte é finalmente iniciar a criação de usuário, clicando no botão superior direito, `Criar usuário`.
<div align="center"> <img src="https://github.com/bmsousa9/CompassUOL-Semana-05/assets/111213549/512bf3d6-98f4-4797-b0df-dc4e23f36c97"/> </div>

O próximo, é nomear o usuário. Nesse caso, nomeei para `terraform`. Logo em seguida criei uma senha para esse usuário.
<div align="center"> <img src="https://github.com/bmsousa9/CompassUOL-Semana-05/assets/111213549/64b760f6-de5e-4090-9e93-2bd6c54b6798"/> </div>
<div align="center"> <img src="https://github.com/bmsousa9/CompassUOL-Semana-05/assets/111213549/d26ee3c3-aa11-4939-971f-0f75d868ef06"/> </div>

Como é uma conta recém criada e sem grupos de usuários, tratei de criar um grupo chamado `Terraform-EC2-Group` liberando acesso total ao gerenciamento e criação das EC2 `AmazonEC2FullAccess`.
<div align="center"> <img src="https://github.com/bmsousa9/CompassUOL-Semana-05/assets/111213549/344e845a-522b-47b1-ba52-c0dd047b6823"/> </div>
<div align="center"> <img src="https://github.com/bmsousa9/CompassUOL-Semana-05/assets/111213549/3ff88159-27eb-429e-8c5a-0a3cfa24704e"/> </div>
<div align="center"> <img src="https://github.com/bmsousa9/CompassUOL-Semana-05/assets/111213549/ab4f4b35-205f-497e-a319-1a29571126e8"/> </div>

Com o grupo de usuários recém criado, tratei de selecionar e clicar em `próximo`.
<div align="center"> <img src="https://github.com/bmsousa9/CompassUOL-Semana-05/assets/111213549/fec2273c-b9b9-4666-8e81-5bf16e0e9751"/> </div>

Criei uma etiqueta como a chave `origin` e valor `Sprint-05` para entender, futuramente, de onde é esse usuário.
<div align="center"> <img src="https://github.com/bmsousa9/CompassUOL-Semana-05/assets/111213549/a8eb10ad-5171-4f99-8d18-3997c29d9e3c"/> </div>


### Criação das Chaves de Acesso (Access Key) na AWS


Com o usuário `terraform` criado, vamos selecionar o usuário recentemente criado.
<div align="center"> <img src="https://github.com/bmsousa9/CompassUOL-Semana-05/assets/111213549/251dfb6f-363f-4e0e-9ece-3f016936a654"/> </div>

A partir daí, selecionei `Command Line Interface (CLI)` e cliquei em `Avançar`.
<div align="center"> <img src="https://github.com/bmsousa9/CompassUOL-Semana-05/assets/111213549/503a1743-320d-4b03-9643-338b832292c0"/> </div>

Logo em seguida, criei mais uma etiqueta `terraform-key`.
<div align="center"> <img src="https://github.com/bmsousa9/CompassUOL-Semana-05/assets/111213549/eeded8a6-3612-4e46-a757-7b3f76fa9757"/> </div>

Com esses passos temos a `Access Key` e `Secret Access Key` devidamente criados.
<div align="center"> <img src="https://github.com/bmsousa9/CompassUOL-Semana-05/assets/111213549/1c4709e2-5f99-474a-89cf-e651de179d68"/> </div>


### Inserir as Access Key no Powershell


Ao abrir o `Powershell`, digitei o comando `aws configure` e em seguida inseri a `Access Key`, a `Secret Access Key` e defini como região `us-east-1`.
```
aws configure
```
```
[Access Key]
[Secret Access Key]
us-east-1
```
<div align="center"> <img src="https://github.com/bmsousa9/CompassUOL-Semana-05/assets/111213549/bc6de26b-d84f-4f54-86bc-6c2b9c895234"/> </div>


### Usar o Visual Studio Code


ENTRA
```
ENTRA
```
<div align="center"> <img src=""/> </div>

ENTRA
```
ENTRA
```
<div align="center"> <img src=""/> </div>
