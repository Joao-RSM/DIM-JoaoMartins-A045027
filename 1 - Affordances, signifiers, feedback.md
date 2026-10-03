# Análise: Componente de Controlo de Volume

Neste trabalho decidi fazer a análise do componente de controlo de volume, no youtube, como demonstrado nas imagens abaixo:

<div align="center">
  
### Estados do Componente

| Máximo | Meio | Sem Som |
| :---: | :---: | :---: |
| <img width="119" height="50" alt="Volume Máximo" src="https://github.com/user-attachments/assets/af323500-81d1-46e4-9f23-d9a5131c2ed0" /> | <img width="111" height="45" alt="Volume a Meio" src="https://github.com/user-attachments/assets/67788136-b72b-4b78-be81-8e1b6bcd9365" /> | <img width="111" height="45" alt="Sem Som" src="https://github.com/user-attachments/assets/8b4479c2-f0df-4753-a504-d9a312e9d7fc" /> |

</div>

<br>

## Questões da Interface

**Que ações é que o elemento permite de facto?**

Permite ajustar o nível de volume de áudio, definindo a intensidade do som do sistema ou da aplicação.

---

**Que ações parece permitir (affordances)?**

Esta estrutura permite agarrar e arrastar (deslizar o círculo para a esquerda ou direita). O ícone do altifalante é um botão clicável que permite também a ação de silenciar ou ativar o som.

---

**Que signifiers existem?**

* O ícone universal do altifalante adapta-se ao estado do componente: exibe duas ondas sonoras no volume máximo, reduz para uma onda a meio e transforma-se num altifalante com um "x" quando está totalmente sem som.
* O contraste de cor na barra mostra o volume atual: a parte preenchida exibe uma linha branca sólida até ao círculo, enquanto o espaço disponível restante apresenta uma linha cinzenta escura.
* O círculo no final da linha branca atua como um "puxador". No estado sem som, este círculo encontra-se totalmente encostado à esquerda, sinalizando o ponto mínimo da barra e vice-versa no estado de volume máximo.

---

**Algum signifier contraria a forma?**

Sim. A forma de "puxador" sugere que a única forma de utilizar o componente é através do ato de arrastar. Contudo, é possível clicar em qualquer espaço da barra e o volume passa imediatamente para esse ponto.

---

**Que feedback devolve, e quando?**

O feedback é imediato e dinâmico. Visualmente, à medida que se arrasta ou clica, o círculo move-se, a proporção da barra branca e cinzenta altera-se, e o ícone do altifalante atualiza em tempo real. Auditivamente, o som em reprodução acompanha esta variação.

---

**O que acontece quando existe alguma falha?**

Se houver um conflito de hardware (ex: dispositivo de áudio desconectado), o componente mantém-se mas não há reprodução de som.

---

**Funciona sem visão ou sem rato?**

Sim. 
Sem rato, é possível selecionar a componente tecla `Tab` e operar através das setas `←` (diminuir) e `→` (aumentar), além disso, possui atalhos: pressionar a tecla `M` alterna imediatamente o estado do som (mute/unmute), e utilizar as setas Cima `↑` (aumentar) e Baixo `↓` (diminuir) ajusta o volume em incrementos de 5%.

Sem visão, é possível através dos vários atalhos disponibilizados. Ao clicar `↑` ouvimos o volume a aumentar, com `↓` o volume a diminuir e com `M` a dar mute/unmute no som.
