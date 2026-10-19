# Análise: Interface Frustrante - IMT Online

Neste trabalho decidi fazer a análise de uma interface que considero insatisfatória e frustrante: o portal IMT Online, nomeadamente no processo de renovação da carta de condução e submissão de atestados, como demonstrado na imagem abaixo:

<div align="center">
### Interface de Submissão

| Portal do IMT Online |
| :---: |
| <img width="600" alt="Exemplo do portal IMT Online" src="coloca_aqui_o_link_da_tua_imagem_ou_print" /> |
</div>

<br>

## Questões da Interface

**Que ações é que o elemento permite de facto?**

Permite preencher dados pessoais, anexar documentos (como o atestado médico) e submeter o pedido formal de renovação da carta de condução.

---

**Que ações parece permitir (affordances)?**

Algumas caixas em branco sugerem a introdução de texto. No entanto, muitos botões de ação fundamentais não possuem a *affordance* típica de um botão (ausência de relevo, bordas ou sombras), parecendo apenas blocos de texto estático na página.

---

**Que signifiers existem?**

* O texto (labels) junto aos campos indica o tipo de dado que é esperado (ex: NIF, Código Postal).
* O cursor altera o seu estado (para o ícone da "mãozinha") quando passa por cima de certos elementos de texto, sendo muitas vezes o único *signifier* real de que aquela área é clicável.

---

**Algum signifier contraria a forma?**

Sim. A falta de destaque visual nos botões interativos faz com que a sua forma se assemelhe a texto de leitura. Para além disso, o processo exige várias etapas, mas a ausência de um mapa de progresso visual (*stepper*) contraria a forma como navegamos num fluxo de múltiplas páginas, deixando o utilizador perdido.

---

**Que feedback devolve, e quando?**

O feedback é tardio e ineficaz. O sistema não valida os dados em tempo real enquanto o utilizador escreve. Permite preencher o formulário com erros e só devolve feedback negativo *depois* do clique em submeter. Além disso, no momento do clique, não existe qualquer feedback de carregamento (*spinner* ou barra de progresso), deixando o ecrã estático e o utilizador na dúvida se o clique foi registado.

---

**O que acontece quando existe alguma falha?**

Se houver um erro de preenchimento detetado após a submissão, a página recarrega para apresentar a mensagem de erro, mas frequentemente apaga os restantes dados que já estavam corretos. Se o utilizador demorar a encontrar um ficheiro para anexar, ocorre uma falha de sessão ("timeout") de forma totalmente silenciosa e o sistema força um *logout* sem avisar, perdendo-se todo o progresso.

---

**Funciona sem visão ou sem rato?**

Sem rato, a navegação é possível através da tecla `Tab`, mas o estado de "foco" é frequentemente invisível, tornando difícil para o utilizador perceber visualmente em que campo ou botão se encontra no momento. 

Sem visão, a usabilidade é extremamente pobre. Muitos campos de introdução de dados não estão semanticamente ligados às suas respetivas etiquetas (labels) no código do site. Consequentemente, os leitores de ecrã não conseguem informar de forma clara que informação específica está a
ser pedida em cada caixa.
