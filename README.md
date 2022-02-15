<h1 align="center"> Projeto Semáforo Inclusivo </h1>
<p align="center">
Esse projeto simula basicamente dois semáforos:
um semáforo é utilizado para o trânsito e possui LEDS Verde,Amarelo, Vermelho. O outro semáforo conta com três leds (Verde,Amarelo e Vermelho).
</p>

<p align="center">
Além disso, há o uso de um timer para piscar o led amarelo do semáforo de pedestres algumas vezes, no intuito de avisar que o semáforo vai fechar, além de um botão que serve como entrada de dado e 
simula o próprio botão de um semáforo utilizado pelos pedestres quando querem atravessar a rua. A ideia do timer e do botão é assegurar inclusão, flexibilidade e segurança durante a travessia, principalmente de indivíduos com mobilidade reduzida, como idosos ou pessoas portadores de deficiência.
</p>

<p align="center">
O projeto semáforo inclusivo foi elaborado utilizado o microprocessador STM32F103C6, LEDS, 1 botão e resistores na simulação feita pelo Proteus em conjunto com a programação no STM32CubeIDE.
</p>

<h3 align="center"> Microcontrolador STM32F103C6 </h3>
<div align="center">
<a href="https://ibb.co/kGmYX7N"><img src="https://i.ibb.co/3TRtc3g/STM32-F103-C6.png" alt="STM32-F103-C6" border="0"></a>
</div>

<h3 align="center"> Semáforos utilizados </h3>
<div align="center">
<a href="https://imgbb.com/"><img src="https://i.ibb.co/RzqxtGT/Semaforos-utilizados.png" alt="Semaforos-utilizados" border="0"></a>
<p align="center"> Semáforo de cima é o de trânsito, já o de baixo é o de pedestres </p>
</div>


<h3 align="center"> Botão de controle do semáforo de pedestres </h3>
<div align="center"> 
<a href="https://imgbb.com/"><img src="https://i.ibb.co/D9VF2yR/BOT-O-QUE-CONTROLA-SEMAFORO-DE-PEDESTRES.png" alt="BOT-O-QUE-CONTROLA-SEMAFORO-DE-PEDESTRES" border="0"></a>
</div>

<h3 align="center"> Simulação no Proteus </h3>
<div align="center">
<a href="https://imgbb.com/"><img src="https://i.ibb.co/N6S4hR1/SIMULA-O-PROTEUS.png" alt="SIMULA-O-PROTEUS" border="0"></a>
</div>

<p align="center">
O microcontrolador STM32F103C6 foi configurado no STM32CubeIDE com as devidas GPIO_OUTPUT's (6 para os LEDS e 1 para o botão) e 1 timer que pisca 4 vezes por segundo. Essa configuração pode ser vista abaixo:
</p>

<h3 align="center"> Configurações do microcontrolador STM32F103C6 no STM32CubeIDE </h3>
<div>
<div align="center">
<a href="https://ibb.co/QcWdYY2"><img src="https://i.ibb.co/vBNYLL7/STM32-F103-C6-configurado.png" alt="STM32-F103-C6-configurado" border="0" align="center"></a>
</div>
<ul> 
<li>Led Verde do semáforo de trânsito configurado como GPIOA_Output no pino PA0-WKUP da porta A</li>
<li>Led Amarelo do semáforo de trânsito configurado como GPIO_OUTPUT no pino PA1 da porta A</li>
<li>Led Vermelho do semáforo de trânsito configurado como GPIO_Output no pino PA2 da porta A</li>
<li>Led Verde do semáforo de pedestres configurado como GPIO_Output no pino PB0 da porta B</li>
<li>Led Amarelo do semáforo de trânsito configurado como GPIO_Output no pino PB1 da porta B</li>
<li>Led Vermelho do semáforo de pedestres configurado como GPIO_Output no pino PB2 da porta B</li>
<li>Botão configurado como GPIO_Output no pino PB15 da porta B</li>
</ul>
<br>
<h3 align="center"> Algumas configurações do timer para esse microcontrolador </h3>
<div align="center">
<a href="https://ibb.co/gDgJNhk"><img src="https://i.ibb.co/NLYK5bc/Algumas-configura-es-do-timer-utilizado.png" alt="Algumas-configura-es-do-timer-utilizado" border="0"></a>
</div>
<p>
Lembrando que o timer pisca alternadamente o led amarelo do semáforo de pedestre, até ser interrompido e resetado.
</p>


<p align="left">
<ul>
<li> <a href="https://www.st.com/en/microcontrollers-microprocessors/stm32f103c6.html"> Datasheet do microcontrolador STM32F103C6 </a> </li>
</ul>
</p>

<div align="center">
<p align="center">
O código foi escrito na linguagem C na IDE STM32Cube e foram utilizados comandos que referenciam a biblioteca HAL do STM32
<br>
A lógica do programa é resumida no diagrama de blocos abaixo e se divide basicamente em três casos:
</p>
<h3 align="center"> Lógica da programação do semáforo inclusivo </h3>
<a href="https://ibb.co/QfwmM9v"><img src="https://i.ibb.co/NsBYKx2/DIAGRAMA-OFICIALL.png" alt="DIAGRAMA-OFICIALL" border="0"></a>
</div>
<br>
<ul>
<li> <a href="https://www.st.com/resource/en/user_manual/dm00105879-description-of-stm32f4-hal-and-ll-drivers-stmicroelectronics.pdf"> Referências da biblioteca HAL do STM32 </a> </li>
</ul>

<div align="center">
<p align="center">
A execução de todo o projeto com a introdução e lógica do programa, a explicação do código feito no STM32Cube IDE e a análise da simulação feita no PROTEUS está disponível em:
<h3 align="center"> <a href="https://youtu.be/jaomG8MJksM"> Projeto Semáforo Inclusivo </a> </h3>
</p>
</div>

<p>
Integrantes do projeto:
<ul>
<li>Renan Martins Dantas Reis // Matrícula:496086</li>
<li>Vitor César Dantas Chaves // Matrícula:497477</li>
<li>Vitor Gabriel Nunes Cesarino // Matrícula:496030</li>
</ul>

