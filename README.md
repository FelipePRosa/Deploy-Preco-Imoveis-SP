
[![author](https://img.shields.io/badge/author-FelipeRosa-red.svg)](https://www.linkedin.com/in/felipe-pimentel-rosa-19975b10b/) [![](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/release/python-365/) [![GPLv3 license](https://img.shields.io/badge/License-GPLv3-blue.svg)](http://perso.crans.org/besson/LICENSE.html) [![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/carlosfab/data_science/issues)

<p align="center">
  <img src="banner_FPR.png" >
</p>

# Deploy de Previsão de Preço de Imóveis em São Paulo
<sub>Neste repositório estará listado os passos e as configurações utilizadas para realizar o deploy de um sistema de previsão de preço de imóveis na cidade de São Paulo utiilizando-se de um dataset contendo nformações diversas sbre os imóveis em análise.</sub>

## 1. Criação do modelo
<sub>A modelagem foi feita utilizando o google colab (plataforma de programação em Python que utiliza de um ambiente totalmente online do google) e então foi exportado o resultado para ser utilizado no próximo passo. O código realizado em COlab pode ser visto no seguinte endereço: **Preço de Imóveis em São Paulo:** https://bit.ly/3xiTLvo</sub>

## 2. Criação do Ambiente Flask
<sub>Agora com a modelagem pronta, foi necessário criar o ambiente Flask onde irá rodar a API para prover os resultados. O arquivo App.py contém o código para ciar os métodos <b>Post</b> e <b>Get</b> para que a API possa receber e fornecer as informações de previsão necessárias</sub>

## 3. Deploy do Algorítmo
<sub>Por si só, o algoritmo estaria hospedado na red local, mas para maior funcioalidade e acesso o deploy foi feito com o auxílio do Heroku. Este permite Hospedar a API de forma online para ter acesso web. O deploy no Heroku funciona como um push no git, porém este estará sendo hospdado em funionamento no site, segue o link hospedado: https://murmuring-cove-39309.herokuapp.com/</sub>
<sub>Para isso também é necessário que tanto a biblioteca do Heroku e do Gunicorn Procfile estejam presentes.
* As bibliotecas serão responsáveis pelo entendimento e excução dos comandos encessário para a hospedagem
* O arquivo Procfile irá executar o comndo de servidor do Gunicorn
* <i>Requirements.txt</s> cont´m informação das bibliotecas e suas versões quando o arquivo foi gerado</sub>

## 4. Verificação da API
<sub>Para teste, disparar um post request utilizando qualquer software d interação com API é suficiente. No meu caso fiz o uso do Insomnia e do Postman, a seguir segue a verficação no Insomnia:
  1) Link de hospedagem da API no método Post
![image](https://user-images.githubusercontent.com/80067455/121823087-5723b880-cc79-11eb-9b8e-57a0b0da54ab.png)
  2) Variáveis de entrada do modelo de previsão
![image](https://user-images.githubusercontent.com/80067455/121823143-a23dcb80-cc79-11eb-857b-c186eea56abd.png)
  3) Envio do request
![image](https://user-images.githubusercontent.com/80067455/121823181-dc0ed200-cc79-11eb-973e-62132322b336.png)
  4) Resposta do request enviado
![image](https://user-images.githubusercontent.com/80067455/121823210-1c6e5000-cc7a-11eb-93ac-b0fd535c493d.png)
</sub>

## 5. Publicação GitHub
<sub>Por fim, para manter registro, um outro remote para realizar o push do git foi adicionado, além do Heroku agora no GitHub. Dessa forma os arquivos se mantém atualizaos em seu devido funcioamento</sub>

**Links:**
* [LinkedIn](https://www.linkedin.com/in/felipe-pimentel-rosa-19975b10b/)
* [Medium](https://medium.com/@felipepimentelrosa)


