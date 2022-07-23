# KOTLIN

***Escrevendo primeira linha de código com kotlin***
```kotlin
    fun main() {
        println("Hello world!")
    }
```

***Método main***
```kotlin
    fun main {

    }
```

***Exibindo uma mensagem na tela***
```kotlin
    println("Hello world!")
```

***Variável mutável***
```Kotlin
    var product = "Nome do projeto"
    product = "Smartphone Samsung A01"
    println(product)
```

> ***Variáveis mutáveis permitem mudar o valor contido dentro delas***

***Variável Imutável***
```kotlin
    val product = "Smartphone Samsung A01"
    println(product)
```

> ***Váriáveis imutáveis não permitem mudar o valor contindo na variável***

***Escrevendo comentários***
```kotlin
    // TODO: 22/07/2022  Apredendo a criar comentários

    // Comentário de uma linha

    /*
     Comentário de multiplas linhas
     */

    // Variável Imutável
    val product = "Smartphone Samsung A01"

    // Variável Mutável
    var age = 14
```

***Exibindo o tipo da variável***
```kotlin
    val price = 31.90
    val product = "Smartphone Samsung A01"
    val age = 21
    println(price::class)
    println(product::class)
    println(age::class)
```

> ***Ao colocar o {nome da variável}::class você está pedindo para que seja informado qual é o tipo dessa variável***

***Declarando o tipo da variável***
```kotlin
    val price: Double = 31.90
    val product: String = "Smartphone Samsung A01"
    val age: Int = 21
```

> ***Quando não declaramos o tipo da variável, o Kotlin entende Automaticamente qual é o tipo da variavel com a inferência de tipos, ou seja: Através da dedução de tipos {var name = "Flávio"}***

***Tipos de dados primitivos***
```kotlin
    // TODO: 22/07/2022 GLOSSÁRIO  (Double, Float, String, Int, True, False)

    /*
    Números Decimais
    */

    // Double Espaço de 64-bit ponto-flutuante (floating point)
    val price: Double = 31.90

    // Float Espaço de 32-bit
    val desconto: Float = 10.90f

    /*
    Formato de texto
    */

    // String
    val product: String = "Smartphone Samsung A01"

    /*
    Variáveis do tipo inteiro
    */

    // Byte - Espaço de 8-bit
    val byte: Byte = 8
    // Short - Espaço de 16-bit
    val short: Short = 16
    // Int - Espaço de 32-bit
    val age: Int = 32
    // Long - Para espaços gigantescos 64-bit
    val long: Long = 23321424352983287
    // Reservar todo o restante de espaço da variável
    val reserva: Long = 2389128332737L

    /*
    boolean (TRUE | FALSE)
    */

    // boolean 1 byte (8-bits)
    val boolean = true
```

***Conversão de Tipos Primitivos***
```kotlin
    // TODO: 22/07/2022 Converter Inteiro Para Decimal

    val mediaPreco = 99
    val resposta = mediaPreco.toDouble()
    println(resposta)

    // TODO: 22/07/2022 Converter Decimal Para Inteiro

    val price = 99.9
    val converter = price.toInt()
    println(converter)

    // TODO: 22/07/2022 Converter Decimal Para Long
    val long = 23.344356564
    val converterToLong = long.toLong()
    println(converterToLong)

    // TODO: 22/07/2022 Converter Decimal Para String
    val string = 4345.545
    val converterToString = string.toString()
    println(converterToString)
```

***Números vs. Textos***
```kotlin
    val number = "10"
    val answer = number.toInt()
    // TODO: 22/07/2022 Fazendo conversão de forma indireta através de um valor atribuido
    println(answer)
    // TODO: 22/07/2022 Fazendo conversão de forma direta 
    println(number)

    // TODO: 22/07/2022 Convertendo valor inteiro para String 
    val text = 10
    println("Número covertido: ${text.toString()}")
```

***Usando Número Grandes***

```kotlin
    /*
    O Kotlin permite a utilização do _ no código para uma melhor organição na últilização de números grandes
     */

    val number = 329_842_389_385
    println(number)
```

***Operadores lógicos***
```kotlin
    // Operadores Lógicos(+ - / * !)

    // TODO: 22/07/2022 Soma
    var mais = 21
    mais = mais + 9
    println(mais)

    // TODO: 22/07/2022 Subtração
    var menos = 21
    menos = menos - 9
    println(menos)

    // TODO: 22/07/2022 Multiplicação
    var multiplicacao = 21
    multiplicacao = multiplicacao * 9
    println(multiplicacao)

    // TODO: 22/07/2022 Divisão
    var divisao = 21
    divisao = divisao / 9
    println(divisao)

    // TODO: 22/07/2022 Booleano
    // true | false | (1, 0)
    var boolean = false
    // Exibir estado atual do boolean
    println(boolean)
    // Inverter a lógica
    println(!boolean)
```

***Concatenar***
```kotlin
 // TODO: 22/07/2022 Concatenar dois valores
    var valor = "15"
    println(valor + " Idade do Usuário")
```

***Caracteres especiais***
```kotlin
    val name = "Flávio"
    val sobrenome = "Júnior"
    val pularLina = "\n"
    val tab = "\t"
    println(name + sobrenome)
    println(name + pularLina + sobrenome)
    println(name + tab + sobrenome)
```

***Chars***
```kotlin
    // Uma String é uma sequência de caracteres(chars)

    /*
     Variáveis do Char aceitam apenas um Caractere e devem está declarado apenas com aspas simples, enquanto
     variáveis do Tipo String aceitam várias letras e deve ser declara com aspas compostas
     */

    val char: Char = 'F'
    val String = "dfdfdf"
```

***Acessando propriedades***
```kotlin
    // TODO: 22/07/2022 Acessar propriedades do objeto
    val nome = "Flávio Júnior" // OBJETO=tipo
    val tamanhoNome = nome.length
    println(tamanhoNome)

    // TODO: 22/07/2022 Exibir nome maiúscula
    val nomeMaiusculo = nome.uppercase() // Função que muda o comportamento de um objeto
    println(nomeMaiusculo)

    // TODO: 22/07/2022 Exibir nome minúscula
    val nomeMinusculo = nome.lowercase()
    println(nomeMinusculo)
```

***Formatando textos***
```Kotlin
    // TODO: 22/07/2022 Formatar texto em aspas triplas
    val messagem = """
        Olá Flávio, 
        tudo bem com você? 
        Seu produto chegou!
    """.trimIndent() // Ao utilizar o trimIndent, seu código passa a identar seu código
    println(messagem)

    // TODO: 22/07/2022 Separar o texto por ;
    val csv = """
        Texto 01,
        Texto 02
    """.replaceIndent(";") // Define qual tipo de caractere você deseja exibir na tela
    println(csv)

    // TODO: 22/07/2022 Adicionar vários objetos em uma mesma variável
    val name = "Flávio"
    val age = 21
    println("Olá $name, você tem $age anos")
    //Somar valores
    val more = 9
    println("Olá $name, você tem ${more + age} anos")
```

***Condições Lógicas***
```Kotlin
    /*
    Condições Lógicas
    < Menor
    <= Menor ou igual
    > Maior
    >= Maior ou igual
    ! Negação -> Retorna o valor oposto do esperado
    == Igual
    != Diferente
     */

    val age = 20

    if (age <= 17) {
        println("Você é menor de Idade, Não pode votar!")
    } else if (age >= 18 && age <= 69) {
        println("Você é maior de Idade e está apto a votar!")
    } else {
        println("Você é Idoso! Seu voto é opcional!")
    }
```

***Omitir Código***
```kotlin
    // TODO: 22/07/2022 omitir código
    val number = 10
    if (number >= 20) println("O número informado é maior que 20")
    // Executa o que está a frente do if caso seja chamado, caso contrário ignora o if
    println("O número informado é menor que 20")

    // omitir código através de um if-else
    val numero = 15
    if (number == 15) println("O número informado é igual a 15")
    else println("O número informado é diferente de 15")
```

***Condições Compostas***
```Kotlin
    // Tabela verdade

    //
    // Símbolo -> && E -> Todas as empressões devem voltar como verdadeiro
    // TRUE | TRUE = true
    // TRUE | FALSE = false
    // FALSE | TRUE = false
    // FALSE | FALSE = false

    // Símbolo -> || OU -> Uma das empressões deve retornar como verdadeiro
    // TRUE | TRUE = true
    // TRUE | FALSE = true
    // FALSE | TRUE = true
    // FALSE | FALSE = false

    val price = 49
    val nameProduct = "Teclado"
    if (price == 49 || nameProduct == "Teclado") { // Expressão composta
        println("Sucesso")
    } else{
        println("False")
    }
```

***Comparar Strings***
```Kotlin
    val product00 = "Mac"
    val product01 = "Mac"
    if (product00 == product01) {
        println("Verdadeiro")
    } else {
        println("Falso")
    }
```

***Nullable e Elvis***
```Kotlin
    // Nullable -> Aceita null
    val product: String? = "imac"
    //val product: String? = null

    // TODO: 22/07/2022 Fazendo verificação com if-else
    if (product != null) {
        println(product.length)
    }

    // TODO: 22/07/2022 fazendo verificação de forma direta
    println(product?.length)

    // TODO: 22/07/2022 retorna ou a espressão ou zero
    val con = if (product != null) product.length else 0
        println("o valor $con")

    // TODO: 22/07/2022 Utilizando o operador Elvis
    println(product?.length ?: 0)
```

***Funções e Reutilização de Código***
> ***Functions | Funções, são blocos de códigos reutilizáveis.***

Função main:
```kotlin
    fun main(){
        // Inicia o programa
    }
```

***Formato de uma função***
```kotlin
    fun message(){

    }
```

***O formato de uma função é iniciado pelo "fun", que inicia a função enquanto o "message" é o nome da função. Já os "()" são os parâmetros da função. E o "{}" é onde executa os blocos de código na função.***

***A estrutura "fun message()" é chamada de Declaração, já o "{}" é chmado de Body | Corpo***

***Tipos de retornos***
```Kotlin
    // Extrusão sem retorno
    fun message() {
        println("Olá mundo")
    }

    // Função com retorno
    fun somar(): Int {
        return 2 + 1
    }

    // Função sem retorno, do tipo UNIT
    fun add(): Unit {
        val soma = 3 + 5
        println("Valor da soma $soma")
    }
    // TODO: 22/07/2022 por padrão o Kotlin omite o Unit que por sua vez não é necessário adicionar o UNIT para informar que a extrução retorna nada!
```

***Escopo de Funções***
```kotlin
    fun message() {
        fun warning(){
            println("Atenção!")
            // Funções chamadas internamente dentro de uma função principal
        }
        warning()
    }
```

***Declaração e Corpo de uma Função***
```Kotlin
    // body inline - Função mais enchuta
    fun message() = println("Hello world!")
```

***Parametrizando Funções***
```Kotlin
    fun idade(idade: Int) {
        if (idade <= 17) {
            println("Menor de idade")
        } else if (idade >= 18 && idade <= 69) {
            println("Maior de idade")
        } else {
            println("Idoso")
        }
       // if (idade <= 17) println("Menor de idade") else if (idade >= 18 && idade <= 69) println("Maior de idade") else println("Idoso")
    }
```

***Parâmetros Nomeados***
```Kotlin
    fun main() {
        // Parâmetro nomeado
        idade(idade = 15) // Ao preencher os parâmetros, você pode: Manter os parâmetro, reordenar ou não declara o nome do argumento, passando ele de forma direta
    }

    fun idade(idade: Int) {
        if (idade <= 17) {
            println("Menor de idade")
        } else if (idade >= 18 && idade <= 69) {
            println("Maior de idade")
        } else {
            println("Idoso")
        }
    }
```

***Sobrecarga de Funções***
```Kotlin
fun main() {
    idade(16)
    idade("Flávio", 21)
}

fun idade(idade: Int) {
    println("Minha idade é $idade")
}

fun idade(nome: String, idade: Int) {
    println("Nome: $nome, Idade $idade")
}
```

> ***A sobrecarga de funções permite criar mais de uma função com o mesmo nome porém com parâmetros diferentes***

***Valores Padrões de Uma Função***
```Kotlin
    fun main() {
        // TODO: 22/07/2022 Ao preencher os parametros não é necessário colocar como falso o último parametro
        register("Flávio", "flavio@gmail.com")
        // TODO: 22/07/2022 Caso queira mudar o valor padrão da variavél é necessário preencher o valor da váriavel como true 
        register("Rafael", "rafael@gmail.com", true)
        register("Carol", "carol@gmail.com")
    }

    // TODO: 22/07/2022  Ao colocar dentro do parametro o isAdmin como false ele determina que o valor por padrão é falso 
    fun register(name: String, email: String, isAdmin: Boolean = false) {
        println("Nome de usuário: $name, email: $email")
    }
```

# OOP - ORIENTED OBJECT PROGRAMMING

***DRY - don't repeat yourself***

***Criando uma classe em Kotlin***
```Kotlin
    class User { // Classe
        var name: String = ""

        fun print() {
        println(name.uppercase())
        }
    }
```

***Instanciando uma Classe em Kotlin***
```Kotlin
    val user1 = User() // Objeto
    user1.name = "Flávio"
    user1.print()
```

> ***Uma Classe em Kotlin é iniciada pela palavra reserva "class", já o nome da classe "User", vem logo em seguida. Os "()" são chamados de parâmetros, assim como as funções. A declaração dos atributos, construtores e metódos está dentro do "{}" ou como é chamado: Body***

***Métodos de Alteração (set)***
```Kotlin
    fun main() {
        val user1 = User() // Objeto
        user1.name = "Flávio"
        user1.update("Júnior")
        user1.print()
    }

    class User {
        var name: String = ""

        fun print() {
            println(name.uppercase())
        }

        fun update(newName: String) {
            name = "Olá, $newName! seu nome foi atualizado com sucesso!"
        }
    }
```

***Métodos de busca (get)***
```Kotlin
    class User {
        fun getNameLength(): Int {
            return name.length
        }
    }
```

***Construtores***
```Kotlin
    // OPÇÃO 01 - Sem valor padrão + o construtor explicita
    class User constructor(var name: String = "") {}

    // OPÇÃO 02 - Valor padrão
    class User (var name: String = "") {}

    // OPÇÃO 03 - espera que a construção receba o valor (var)
    class User constructor(var name: String) {}
```

> ***Assim como as variáveis, o Kotlin também cria automaticamente um construtor padrão dentro da classe por inferência***

***Sobrecarga de Construtores***
```Kotlin
    // Construtor criado no projeto
    class User constructor(var name: String, var isAdmin: Boolean) {

        // TODO: 22/07/2022 para executar um subconstructor dentro do constructor principal é necessário colocar o this no subconstructor
        constructor(name: String) : this(name, false)
    }
   
   // Instanciando Constructor
    fun main() {
        val user01 = User("Flávio")
        // TODO: 22/07/2022 Ao utilizar dois constructor com parametros default é opcional preencher o segundo parametro
        val user02 = User("Rafael", true)
    }

```

# REGRAS DE NOMEAÇÃO E ESCRITA NO KOTLIN

> ***CAMEL CASE - É uma regra aplica em variáveis por palavras compostas ou frases, onde cada palavra é iniciada com maiúsculas e unidas sem espaços, excerto a primeira letra depois de da variável {voceTemQueEscreverDessaManeira}*** 

> ***Variáveis sempre devem começar com letra minúscula***

> ***Não é utilizado no Koltin caracteres especiais***

> ***Funções não podem conter o mesmo nome***

> ***Nome de classes começam a primeira letra maiúscula***
