## Trabalho final da disciplina de Aprendizado não supervisionado
## Aplicação de PCA para reconhecimento facial
### Professor Márcio Koch
### Especialização em Data Science - FURB

Optou-se por utilizar o Google Colab para desenvolvimento do trabalho com o intuito de facilitar a execução do algoritmo (Python). Por rodar na plataforma online, não é necessária a instalação de pacotes ou ambientes virtuais.

O notebook do colab está disponível no seguinte link (https://colab.research.google.com/drive/11xovUaNsiy4241wQBKuEuGj9SzzvZb2m?usp=sharing). Uma cópia do mesmo está disponibilizada no git (https://github.com/adrianobertoldi/aprendizado_nao_supervisionado/blob/master/Trabalho_Final_Aprendizado_N%C3%A3o_Supervisionado.ipynb)

O único input que o usuário deverá realizar para rodar o algoritmo é o upload do arquivo "ORL.zip" ao Colab. Para fazer o upload, o usuário deve clicar no ícone da pasta e arrastar o arquivo para dentro do painel. O arquivo "ORL.zip" contém também as imagens extras (Ids de 401 a 410). Optou-se por utilizar a imagem de uma figura pública pois a ideia era pegar diferentes configurações de um mesmo rosto, tais como o envelhecimento, uso de barba, posição, óculos, entre outros. O link para o arquivo está em (https://github.com/adrianobertoldi/aprendizado_nao_supervisionado/blob/master/ORL.zip)

Para desenvolvimento do algoritmo, procurou-se utilizar a abordagem mais simples possível. Com isso evitou-se o uso de ferramentas prontas (OpenCV) ou de outros módulos.

Os resultados obtidos na melhor das variantes (usando OpenCV nos cálculos de eigenvectors) são apresentados abaixo:

10 componentes principais, acurácia: 30.9%
11 componentes principais, acurácia: 30.9%
12 componentes principais, acurácia: 31.7%
13 componentes principais, acurácia: 31.7%
14 componentes principais, acurácia: 31.7%
15 componentes principais, acurácia: 31.7%
16 componentes principais, acurácia: 31.7%
17 componentes principais, acurácia: 31.7%
18 componentes principais, acurácia: 31.7%
19 componentes principais, acurácia: 31.7%
20 componentes principais, acurácia: 31.7% 

É possível verificar que esse resultado ficou muito abaixo do apresentado pelo algoritmo desenvolvido em sala (Java). Isso pode ter ocorrido por baixa eficiência nas ferramentas empregadas nesse código ou eventualmente um erro na escrita do algoritmo, não detectado até o momento. Outra hipótese pode recair sobre o uso das imagens selecionadas, onde as mesmas podem ter influenciado o modelo como um todo (imagens fora dos padrões). Assim, para que uma versão de produção seja desenvolvida, serão necessários ajustes e correções no algoritmo proposto. 