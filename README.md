
# _Projeto Machine Learning Microsoft Azure - modelo de previsão com pontos de extremidade definidos no caso de aluguel de bicicletas_ 

Segue abaixo os passos definidos para realização do projeto

## Criando espaço de trabalho no Machine Learning Microsoft Azure

1 - Primeiro passo, acessar o [Microsoft Azure](https://portal.azure.com) usando os dados de sua conta e, após isso, criar um recurso no Microsoft Azure através de "Create Resource".

2 - Procurar por Azure Machine Learning e criar um espaço de trabalho.

3- Será solicitado subscription e resource group (onde será feita toda a configuração do espaço de trabalho) e também o nome.

4- Para validar, pressionar "Review+create". E depois, "create". (Pode demorar um tempo, pois o Azure estará processando as informações
mostrando a mensagem "Deployment is in progress"). Depois de finalizado, surgirá a mensagem "your deployment is complete".

## Configurar modelos e conjunto de dados

5 - Depois de finalizado o processo, clicamos em "Go to resource"

6 - Por conseguinte, clicar em "Launch Studio", que direcionará para a página https://ml.azure.com.

7 - Na barra da esquerda, na sessão "criação", acessar "ML automatizado".

8 - Depois, selecionar "Novo trabalho de ML automatizado".

9 - Todas as configurações que serão feitas, utilizará as informações presentes na seguinte [documentação](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/01-machine-learning.html). Utilzando como base de dados https://aka.ms/bike-rentals.

10 - Após realizar todas as configurações, deverá ser enviado o trabalho para treinamento, pressionando "Enviar trabalho de treinamento" para exame.

11 - No começo o status da análise aparecerá como "não iniciado". Depois, "em execução". Ao finalizar, aparecerá "concluído".
Segue exemplo abaixo:

![image](https://github.com/vgastaldelli/LABORATORIOAZUREAI900-MACHINELEARNING---ALUGUEL-DE-BICICLETAS/assets/160192109/bd0318b8-7dca-4f06-a99a-ba2f427aefba)

## Definição de modelo e pontos de extremidade

12 - Primeiro acessar a aba "Modelos" na aba esquerda e escolher opção "Registrar modelo de uma saída de trabalho". Seguindo 
os passos presentes na [documentação](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/01-machine-learning.html)

13- Depois para definição dos pontos de extremidade, selecionar a aba "ponto de extremidade" e selecionar o modelo criado anteriormente 
"predict-rentals".

14 - Após "bem-sucedido", deverá testar. Na aba "pontos de extremidade em tempo real" clicar em "teste" e deverá substituir os dados pelo do template JSON contido na [documentação](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/01-machine-learning.html), no campo "Input".

15 - Por fim, testado, aparecerá o "jsonOutput", que inclui um número previsto de aluguéis com base nos recursos de entrada. 
Segue exemplo abaixo:

![Jsonoutput](https://github.com/vgastaldelli/LABORATORIOAZUREAI900-MACHINELEARNING---ALUGUEL-DE-BICICLETAS/assets/160192109/0d3452c7-e644-4e49-b105-d36d78957bb1)
