# React_aula09
<h1>Aprendizados da aula </h1>

<p>Nesta aula foi criado um componente chamado Menu dentro do arquivo MenuComponent.js. Este componente terá os dados de pratos
disponibilizados por um estado chamado "dishes" que possuí um array de objetos contendo os pratos.</p>

<h2>Diretório do component</h2>

![alt text](02.png)

<h2>Diretório das imagens</h2>

![alt text](02A.png)

<h2>Códigos </h2>

![alt text](01.png)

![alt text](01A.png)

![alt text](01B.png)

<p>Após exportar o componente com "export default menu", esse componente precisa ser importado no App.js . Depois ele precisa ser chamado com o comando "< Menu />"</p>

![alt text](02B.png)


<h2>MeuComponent.js</h2>
<h3>Quais os imports utilizados?</h3>
<p>React: Possuí todos os componentes básicos do react.</p>
<p>UseState: Gerencia os estado dos dados, ele contém o valor atual, podendo ser alterado com o tempo, ele faz isso através de um componente que retorna um array contendo o valor atual e uma função para atualizar o valor .</p>
<h3>Há componentes? o que fazem?</h3>
<p>Existe o componente menu, esse componente irá exibir os pratos.</p>
<h3>Para que serve o onDishSelect no projeto?</h3>
<p>Nessa função, quando o usuário clicar no prato(dish) em questão e atualiza o estado do componente "selectedDish"</p>
<h3>Para que serve o renderDish?</h3>
<p>Recebendo o prato(dish) como argumento,essa função, caso o valor de prato
não seja nulo, irá retornar um componente "card" contendo a imagem juntamente com as demias informações desse prato</p>
<h3>Para que serve o props.dishes.map?</h3>
<p>Essa função itera sobre cada prato no array e retornará um novo componente para cada prato. Ao clicar na imagem para um "div" abaixo dos demais card, um card contendo a imagem e as demais informações dos pratos</p>
<h3>Quais as propriedades?</h3>
<ul>
<li>id</li>
<li>name</li>
<li>image</li>
<li>category</li>
<li>price</li>
<li>description</li>
<li>comments: Este é um array que tem as seguintes propriedades:id,rating,comment,author,date.</li>
</ul>
<h3>Qual tipo de date é utilizado?</h3>
<p>O date utilizado é o ISO 8601 e ele é usado para facilitar o processamento e a comparação de datas e horas em diferentes sistemas e linguagens de programação.</p>
<h3>Para que serve oconst [dishes]?</h3>
<p>Essa linha de código utiliza o hook useState do React para criar um estado local chamado dishes. O estado é essencial para gerenciar dados que podem mudar ao longo do tempo, como no caso dos pratos do restaurante.

Aqui, o estado dishes é inicializado com o valor do array DISHES, que é importado do arquivo shared/dishes. Isso significa que, inicialmente, o componente App terá acesso a todos os pratos definidos em DISHES.</p>

<h3>Como funciona o "Menu dishes={dishes} /" ?</h3>
<p>Este código renderiza um componente chamado Menu e passa a ele uma propriedade chamada dishes. Essa propriedade contém o array de pratos que foi definido no estado do componente App.

O componente Menu provavelmente recebe essa propriedade dishes e a utiliza para renderizar uma lista de pratos na tela. Isso pode envolver:

Iterar sobre o array de pratos.
Renderizar um item de menu para cada prato.
Exibir informações como o nome, imagem, descrição e preço de cada prato.
Possivelmente, implementar funcionalidades como filtros, ordenação ou busca de pratos.
Em resumo, o componente Menu recebe os dados dos pratos do componente App através da propriedade dishes e os utiliza para criar a interface de usuário que mostra esses pratos ao usuário.</p>