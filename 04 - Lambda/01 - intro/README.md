# Aula 02.1 - Lambda


1. No terminal do IDE criado no cloud9 execute o comando `cd ~/environment/fiap-cloud-computing-tutorials/04\ -\ Lambda/01\ -\ intro/` para entrar na pasta que fara este exercicio.
 2. Iniciar o repositório de trabalho `sls create --template "aws-python3"`
 ![img/slscreate.png](img/slscreate.png)
 3. Execute o comando `npm install -g serverless-pseudo-parameters` para instalar o plugin necessário para essa stack.
 4. Explore os arquivos criados(serverless.yml e handler.py) pelo comando anterior utilizando o menu de navegação lateral:
    ![img/explore.png](img/explore.png)
 5. Abra o arquivo serverless.yml no IDE com o comando `c9 open serverless.yml`
 6. Altere o arquivo para que fique como na imagem abaixo. Para salvar utilize CTRL+S.
   ![](img/yml1.png)
 7. No terminal do IDE faça deploy da função criada com o comando `sls deploy`
 ![img/slsdeploy.png](img/slsdeploy.png)
 8. Testar remotamente a função `sls invoke -f hello`
![img/slsinvoke.png](img/slsinvoke.png)
 9. Altere a versão do retorno da função para 1.1 no arquivo "handler.py" como na imagem e salve com as teclas "CTRL + S"
   ![img/altereversao.png](img/altereversao.png)
 10. Faça um teste local da sua função no terminal com o comando `sls invoke local -f hello` 
![img/slsinvokelocal.png](img/slsinvokelocal.png)
 11. Para deletar a função que esta no lambda utilize o comando `sls remove`
![img/slsremove.png](img/slsremove.png)
