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

 A partir daí recebi um e-mail com o código de verificação que foi necessário para continuar com a criação da senha e da conta. Nos passos seguintes, é necessário a inserção de um cartão de crédito válido, de um número de celular válido e fazer novamente a verificação.
 <div align="center"> <img src="https://github.com/bmsousa9/CompassUOL-Semana-05/assets/111213549/25aed3b5-3099-4e3b-8c46-a51743bd3af6"/> </div>

Com esses passos, foi possível ter acesso ao console da AWS.
<div align="center"> <img src="https://github.com/bmsousa9/CompassUOL-Semana-05/assets/111213549/fe6ae9ff-4d93-43bc-b584-4514933d1011"/> </div>


### Criação de um usuário AWS AMI

No console da AWS, digitei 
<div align="center"> <img src=""/> </div>

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

ENTRA
```
ENTRA
```
<div align="center"> <img src=""/> </div>





