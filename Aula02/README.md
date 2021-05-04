# Conceitos básicos de forma aprofundada

### Este é o material complementar da primeira aula do curso básico de Ruby feito pelo Arthur Ottoni no YouTube. 

#### Conteúdos desta aula:

* conversion
* strings
* gets & chomp
* if, else & elsif

###### Se inscreva no canal do YouTube (no fim do artigo) para assistir as aulas referentes ao curso!

# Conceitos básicos de forma aprofundada

### Conversion

* **to_s:** Converte valor para o tipo: String
* **to_i:** Converte valor para o tipo: Integer
* **to_f:** Converte valor para o tipo: Float

```ruby
Nome = "Rafaella"
Sorte = 77
Aleatorio = 14.5

Sorte.to_s # Transformará em "77"
Aleatorio.to_i # Transformará em 14
Nome.to_f ou Nome.to_i # Transformará em 0.0 // 0
```

### Strings de forma aprofundada

#### Utilizar métodos em nossas strings podem facilitar diversas coisas, como as validações que faremos no final da aula. 

**Métodos utilizados em strings:**

* **variavel.length():** Retorna a quantidade de caracteres.
* **variavel.slice(numero):** Retorna a posição de algum caractere ou uma area. Ex: variavel.slice(4) ou variavel.slice(1,3)
* **variavel.upcase:** Retorna a string totalmente em maiuscula.
* **variavel.downcase:** Retorna a string totalmente em minuscula.
* **variavel.empty?:** Retorna se a string é vazia (boolean).
* **variavel.include 'palavra':** Retorna se contém tal string dentro da variavel.
* **variavel.reverse:** Retorna a string de forma reversa.

```ruby
string = "Esta é uma string!" # declaraao de uma variável recebendo uma string como valor

puts string.length() # retorna a quantidade de caracteres
puts string.slice(0, 3) # retorna a posição de algum caractere ou uma area

puts string.upcase # retorna a string totalmente em maiuscula
puts string.downcase # retorna a string totalmente em minuscula
puts string.empty? # retorna se a string é vazia (boolean)
puts string.include? 'ruby' # retorna se contém tal string dentro da variavel string
puts string.reverse # retorna a string de forma reversa

```

###### Pesquisem mais métodos!


### gets & chomp

#### Utilizamos os métodos gets e chomp para receber dados pelo usuário, sendo assim, ele fará o papel de *input* de dados.

* **Vamos ver a utilização do gets.chomp na prática:**

```ruby
print "Digite seu nome: "
nome = gets.chomp

puts nome # Irá retornar o nome digitado pelo usuário
```
* **Agora que entendemos o funcionamento, podemos completar ele utilizando a *convertion***

```ruby
print "Digite seu nome: "
nome = gets.chomp.to_s # Recebe os dados digitados e transfora para string
print "Digite sua idade: "
idade = gets.chomp.to_i # Recebe os dados digitados e transfora para integer

puts "Olá #{nome}, você tem #{idade} anos" # Retornará as variáveis com interpolação.
```

###### Caso não saiba o que é interpolação, volte na primeira aula!

### If, Else & Elsif

#### São estruturas condicionais, ou seja, verificam uma condição (true or false).

* **if:** Verifica se a condição é verdadeira. (caso seja, executará algo)

* **elsif:** Verifica se outra condição é verdadeira. (caso seja, executará algo)

* **else:** Verifica se as condições do if e elsif são falsas. (caso seja, executará algo)

  ```ruby
  nome = "Arthur"
  
  if nome == "Arthur" # Verifica se nome é igual a "Arthur"
      puts "Olá arthur" 
  elsif nome == "Rafaella" # Verifica se nome é igual a "Rafaella"
      puts "Olá Rafa"
  else # Caso nenhuma alternativa seja verdade será executado
      puts "Nome não reconhecido"
  end
  
  ```

###### É necessário o uso do "end" e que condições de igualdade sejam representadas com "==". Tentem o uso de apenas "=" e sem o end para verem os erros e aprenderem!  

######  

---

## About me

* Youtube channel: <a href="https://www.youtube.com/channel/UCQxsPy4aLwGQ9fjZhsDJ70Q" target="_blank">Click Here</a>
* Instagram: <a href="https://www.instagram.com/ottoni.arthur" target="_blank">Click Here</a>
