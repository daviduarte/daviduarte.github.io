# Projects


## Deep Learning Based Digital Breast Tomosynthesis Reconstrction
I developed a [new tool](https://github.com/daviduarte/DBTProjectionsNoiseDiscovery) to generate Digital Breast Tomosynthesis images from a set of projections. This software is the result of my master thesis. I implemented the well-known algorithm in medical imaging litarature named Filtered Backprojection in the form of a Neural Network layer, using Tensorflow. For that, I had to create a new operation in Tensorflow, using its low-level API. I used GPU to became this operation efficient (using CUDA Kernels). In this project, I worked directly with Deep Learning, Tensorflow (efficient operations implementations using GPGPU), theorical computer vision concepts like image processing, image synthesis, projection matrices and noise filtering.

//Eu implementei o algoritmo de reconstrução bem conhecido na literatura médica chamado de Retroprojeção Filtrada na forma de uma camada, no Tensorflow. Para isso, precisei criar uma operação nova no Tensorflow utilizando diretamente a sua API de baixo nível. Eu tornei esta operação eficiente usando GPU (utilizando CUDA Kernels). Trabalhei diretamente com conceitos teóricos de visão computacional e processamento de imagens (síntese de imagens, matrizes de projeção, perspectivas, filtragem de ruído, simulação de ruído, etc) e Deep Learning (Tensorflow, implementação de operações eficiente usando GPGPU).

![Image](images/dbt.png)

## CamNuvem - Artificial Inteligence Based Video Surveillance
[In this project](https://camnuvem.com.br) I developed a online platform that allow users connect their surveillance cameras to have their images stored in the cloud and analyzed in real time by Artificial Intelligence, that notify them in WhatsApp if someone ou something exceed a predetermined perimeter in the camera. This tool was tested with real customers and proved to be functional. I used Tensorflow and a pre-treined object detection model. I used a parallel thread to run the object detection model to efficiently process the hundreds of frames per second that customers cameras place in a FIFO.
![Image](images/cerca_virtual.mp4)


//[Neste projeto](https://camnuvem.com.br), desenvolvi uma plataforma online que permite aos usuários conectar câmeras de vigilância para terem suas imagens armazenadas em nuvem e analisadas em tempo real por uma Inteligência Artificial, que os notificam via WhatsApp caso alguém ou alguma coisa ultrapasse um perímetro pré-especificado em suas casas, lojas, empresas, etc. Esta ferramenta foi testada com clientes reais e se mostrou funcional. Utilizei Tensorflow com o modelo de detecção de objetos pré-treinado. Utilizei uma Thread paralela para rodar o modelo de detecção de objetos e processar de forma eficiente as centenas de frames que as câmeras dos usuários depositam a cada segundo em uma FIFO. 

## CamNuvem Distributed Inference
[Neste projeto](https://github.com/daviduarte/distributed_inference) No desenvolvimento da CamNuvem, eu percebi que uma GPU era muito custosa para processar as imagens dos meus clientes. Dessa maneira, eu verifiquei que utilizando várias máquinas simples (1vCPU e sem GPU) era mais barato que a utilização de uma máquina robusta com GPU (utilizando os modelos pré-treinados do Tensorflow Zoo, cujos dados são compostos por ponto flutuante). Assim, eu desenvolvi este projeto, que distribui a inferência de um modelo de Machine Learning (utilizando Tensorflow) em uma rede de dispositivos heterogênios. Assim, eu pude baratear os custos aos meus clientes. Neste projeto eu utilizei conceitos de computação distribuida, como os Relógios Lógicos de Lamport (para sincronizar os frames das câmeras) em uma arquitetura cliente-servidor, além de bibliotecas em python para intercominicação de processos ().
![Image](images/distributed.png)

## Data Analysis in Motocycles Ads
In this project, I implement a Web Scrapper and a Linear Regression Model to analyse the motocycle classified ads in the OLX.com.br (platform widely used in Brazil) to find good deals. The construction of this tool is [detailed here](https://medium.com/ensinando-m%C3%A1quinas/coleta-e-an%C3%A1lise-de-dados-de-motos-no-olx-6d0fd914853b).
![Image](images/olx_data_science.png)

## IA based Snake Game 
In this project, I implement the Snake Game that plays automatically. I used a Fully Connected Artificial Neural Network (FCANN) as the model and Genetic Algorithm to find the best weights of the FCANN. The result and more details can be found in my [YouTube channel](https://youtu.be/0WVAWjVOygE)
![Image](images/snake.png)
