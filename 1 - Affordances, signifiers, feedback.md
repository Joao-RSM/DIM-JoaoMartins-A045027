# Análise: Componente de Controlo de Volume

Neste exercício, analisamos as qualidades de interação — *affordances*, *signifiers* e feedback — do componente de controlo de volume, observando os seus diferentes estados.

<div align="center">

### Estados do Componente

| Máximo | Meio | Sem Som |
| :---: | :---: | :---: |
| <img width="119" height="50" alt="Volume Máximo" src="https://github.com/user-attachments/assets/af323500-81d1-46e4-9f23-d9a5131c2ed0" /> | <img width="111" height="45" alt="Volume a Meio" src="https://github.com/user-attachments/assets/67788136-b72b-4b78-be81-8e1b6bcd9365" /> | <img width="111" height="45" alt="Sem Som" src="https://github.com/user-attachments/assets/8b4479c2-f0df-4753-a504-d9a312e9d7fc" /> |

</div>
<br>

## Questões da Interface

**Que ações é que o elemento permite de facto?**

Permite ajustar o nível de volume de áudio ao longo de um intervalo contínuo, definindo a intensidade do som do sistema ou da aplicação.

---

**Que ações parece permitir (affordances)?**

A sua forma encapsulada em "pílula" revela um eixo horizontal e um botão circular na extremidade da linha branca. Esta estrutura oferece a clara *affordance* de agarrar e arrastar (deslizar o círculo para a esquerda ou direita). O ícone do altifalante sugere também a *affordance* de ser um botão clicável (mutar/desmutar).

---

**Que signifiers existem?**

* O ícone universal do altifalante adapta-se ao estado do componente: exibe múltiplas ondas sonoras no volume máximo, reduz para uma onda a meio e transforma-se num altifalante com um "x" quando está totalmente sem som.
* O contraste de cor na barra demarca o volume atual: a parte preenchida exibe uma linha branca sólida até ao círculo, enquanto o espaço disponível restante apresenta uma linha cinzenta escura.
* O círculo saliente no final da linha branca atua como um "puxador" visual. No estado sem som, este círculo encontra-se totalmente encostado à esquerda, sinalizando o ponto mínimo de interação.

---

**Algum signifier contraria a forma?**

Sim. A forma de calha com um "puxador" sugere fortemente que a única forma de operar o componente é através do ato mecânico de arrastar. Contudo, na interação digital, é possível dar um simples toque ou clique no espaço vazio e o volume salta instantaneamente para esse ponto. A forma física sugere um percurso contínuo, enquanto a interface permite atalhos invisíveis.

---

**Que feedback devolve, e quando?**

O feedback é imediato e dinâmico. Visualmente, à medida que se arrasta ou clica, o círculo move-se, a proporção da barra branca e cinzenta altera-se, e o ícone do altifalante atualiza os seus traços em tempo real. Auditivamente, o som em reprodução acompanha esta variação de forma síncrona.

---

**O que acontece quando existe alguma falha?**

Se houver um conflito de hardware (ex: dispositivo de áudio desconectado), o componente perde geralmente o seu estado ativo (as partes brancas ficam cinzentas/esbatidas) e o manípulo deixa de responder ao cursor, sinalizando a revogação da funcionalidade.

---

**Funciona sem visão ou sem rato?**

Sim, assumindo boas práticas de código. Sem rato, é focado com a tecla `Tab` e operado através das setas `Esquerda` e `Direita`. Sem visão, os leitores de ecrã identificam-no semanticamente e ditam os valores numéricos à medida que são ajustados pelo utilizador.
