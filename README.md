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

***Somar um segundo valor dentro de outra variável com valor definido***
```Kotlin
    fun main() {
        val number = 27
        println(number.plus(54))
    }
```

***Bloco init***
```Kotlin
    init {
        
    }
```

***Acessando propriedades de um objeto***
```Kotlin
    fun main() {
        var name = User1("Flávio")
        println(name.label)
    }

    class User1(var name: String) {
         var label = "Seu nome é ${name}"
    }
```
> ***O bloco init é usado no Kotlin quando queremos iniciar alguma coisa dentro de um Construtor***

***Const em Kotlin***
```Kotlin
    const val MESSAGE = "Warning" // Cria uma constante em tempo de copilação e a a inicia com o valor padrão definido
```
> ***A diferença entre uma const é que ela é criada em tempo de copilação e é inicia com o valor padrão definido enquanto o val é criado em tempo de execução e necessita de um valor que seja atribuido a ela.***

***companion object***
```Kotlin
    class User(var name: String) {

        companion object{ // Corresponde as propriedades e comportamentos da classe

        }

    }
```

***Mudar estado da classe***
```Kotlin
fun main() {
    var name = User1("Flávio")
    User1.resetName() // Para mudar o estado da classe pode ser feita de forma direta, sem a necessidade de instanciar um objeto e acessar sua propriedade
}

class User1(var name: String) {

    companion object {
        var message = "Warning"

        fun resetName() {
            message = ""
        }

    }

}
```

***Singletons***
```Kotlin
    // TODO: 23/07/2022 Objeto único - Instância única que não existe outra instância desse objeto na aplicação | Singletons
    object Formated {
        const val MAX_NAME_LENGHT = 8
        const val PATH = "/Images/"
        const val FORMAT_EXT = ".jpg"
        const val DOMAIN = "https://xvideos.com"
    }
```

***lateinit***
```Kotlin
    fun main() {
        val usuario = Usuario()
        usuario.name = "Flávio"
        usuario.print()
    }

    class Usuario() {
        // TODO: 23/07/2022 Diferente do var e do val o lateinit é iniciada apenas no futuro, ou melhor: Quando for chamada para executar alguma coisa
        lateinit var name: String

        fun print() = println("Meu nome é: $name")

    }
```

***Classes Aninhadas (Nested Class)***
```Kotlin
    fun main() {
        val carro = Carro()
        carro.desc()
        val info = Carro.Dono()
        info.info()
    }

    class Carro() {

        val marca: String = "Fiat"
        val modelo: String = "Fiat Uno 2021"
        val placa: String = "43rsdlk"

        fun desc() = println("Veiculo da Marca: $marca, \n cujo modelo é o: $modelo \n com o número da placa: $placa")

        // TODO: 24/07/2022 Classe associada a outra classe

        class Dono() {
            val nome: String = "Flávio"
            val cpf: String = "123.456.789-10"
            fun info() = println("Dono do veiculo: $nome, \n Número do cpf: $cpf")
        }

    }
```
***Classes Internas (Inner Class)***
```Kotlin
    fun main() {
        // TODO: 24/07/2022 Primeiro instanciar um objeto e depois acessar o segundo metódo da classe e fazer a chamada  
        val motorista = Carro()
        val info = motorista.Dono()
        println(info.info())
    }

    class Carro() {
        val marca: String = "Fiat"
        val modelo: String = "Fiat Uno 2021"
        val placa: String = "43rsdlk"
        val cidade: String = "Buíque-PE"

        // TODO: 24/07/2022 Através do inner class é possivel acessar as propriedades da class de forma interna
        inner class Dono() {
            val nome: String = "Flávio"
            val cpf: String = "123.456.789-10"
            fun info() =
                println(" Senhor: $nome, seu Veículo é o da marca, $marca?, \\n cujo modelo é o: $modelo \\n com de placa: $placa, \\n da cidade de: $cidade\"")
        }

    }
```

***Classes Enumeradas***
```Kotlin
    fun main() {
        // TODO: 24/07/2022  Exibir propriedade da bandeira
        println(CreditCard.VISA)
        // TODO: 24/07/2022 Acessar enumerador da classe
        println(CreditCard.AMEX.ordinal)
        // TODO: 24/07/2022 Buscar propriedade com valor definido
        val creditCardAPIName = "elo"
        val card = CreditCard.valueOf(creditCardAPIName.uppercase())
        println(card)
        // TODO: 24/07/2022 Fazendo comparações
        if (card == CreditCard.VISA) {
            println("Você recebeu um desconto de 30%!")
        } else {
            println("Ao utilizar o cartão visão você tem descontos em nossos produtos!")
            // TODO: 24/07/2022 Acessa as propriedades do objeto
            println("Você está utilizando o cartão: ${card.label}")
        }
    }

    /*
    // TODO: 24/07/2022 Classes Enumeradas

    enum class CreditCard {
        // TODO: 24/07/2022 Ao definir uma propriedade na classe, ela é enumerada Automaticamente!
        VISA,
        MASTER,
        ELO,
        AMEX
    }

     */

    // TODO: 24/07/2022 Classe Enumerada com contrutor

    enum class CreditCard(val label: String) {
        // TODO: 24/07/2022 Ao definir uma propriedade na classe, ela é enumerada Automaticamente!
        VISA("Visa"), // Objeto
        MASTER("Matercard"),
        ELO("Elo"),
        AMEX("American Express")
    }
```

***Condição When***
```Kotlin

    // TODO: 24/07/2022 Quando | When
    val name = "Flávio"

    // TODO: 24/07/2022 Primeira forma de criar um if utilizando o when
    when (name) { // else if
        "Flávio" -> {
            println("Usuário encontrado no banco de dados com Sucesso!")
        }

        else -> println("O usuário informado não existe no banco de dados!") // Função inline

    }

    // TODO: 24/07/2022 Segunda forma de criar um if utilizando o when

    // TODO: 24/07/2022  A IDE sugere que você também possa utilizar no lugar do "name == Flávio" da seguinte forma:
    /*
    *  when (name) {
        "Flávio" ->
    * */
    when {
        name == "Flávio" -> println("Usuário encontrado no banco de dados com Sucesso!")
        else -> println("O usuário informado não existe no banco de dados!") // Função inline
    }
    
    // TODO: 24/07/2022 deixando mais claro o exemplo do uso do when 
    fun main() {

    val card = "Elo".uppercase()
    val marca = CreditCard.valueOf(card.uppercase())
    when (marca) {
        CreditCard.VISA -> println("Você ganhou um desconto")
        else -> println("Ao utilizar o Cartão VISA, você tem desconto de 30% em nossos produtos!")
    }

    }

    enum class CreditCard {
    VISA,
    MASTER,
    ELO,
    AMEX
    }
```

***Retornos encurtados***
```Kotlin
    fun main() {
        val card = "ELO".uppercase()
        val marca = CreditCard.valueOf(card.uppercase())

        // TODO: 24/07/2022 Retornos encurtados com if else
        /*
        val discount =
            if (marca == CreditCard.VISA) {
                "Desconto de 30%"
            } else if (marca == CreditCard.MASTER) {
                "Desconto de 20%"
            } else {
                "Sem desconto"
            }
        println(discount)*/

        // TODO: 24/07/2022 Retornos encutados com when
       val  discount = when (marca) {
            CreditCard.VISA -> "Desconto de 30%"
            CreditCard.MASTER -> "Desconto de 20%"
            else -> "Sem desconto"
        }

        println(discount)
    }

    enum class CreditCard {
        VISA,
        MASTER,
        ELO,
        AMEX
    }
```

***Data class: Classes de Dados***
```Kotlin
     fun main() {
        val user1 = Usuario("Flávio", "juniorflavio.ofc@gmail.com")
        println(user1.name)

        /*

        Caso, estivessimos utilizando o class em vez do data class mesmo o user1 sendo igual ao user dois, o if 
        irá retornar com o valor como falso porque os objetos criados são diferentes quando utilizamos o class, enquanto
        o data class trata os dados como sendo igual

        val user2 = Usuario("Flávio", "juniorflavio.ofc@gmail.com")
        println(user2.name)
        if (user1 == user2) {
            println("Verdadeiro")
        } else {
            println("Falso")
        } 
            */
    }

    /*
    * Diferente das demais classes, o data class, trata as propriedades e cortamentos da classe como dados | Data class: Classes de Dados
    * */
    data class Usuario(var name: String, var email: String)

    /*
    Quando não definimos o tipo da variável, como var ou val não é possivel acessar a propriedade dessa variável
    ao instanciamos a classe, não será possivel acessar os atributos da classe e chamar a variável desejada
    data class Usuario(name: String, email: String)
     */
```

***Desestruturação de Classes***
```Kotlin
    fun main() {
        val user1 = Usuario("Flávio", "flavio@outlook.com")
        val (name, email) = user1 // Ao criamos um variável instanciando o objeto criado, referenciamos o nome, e o email de acordo com a ordem que declaramos o objeto
        println("Nome de usuário: $name, email: $email")
    }

    // TODO: 24/07/2022 A Desestruturação de Classes é possivél apenas utilizando data class
    data class Usuario(var name: String, var email: String)
```

***Copiando Objetos no Kotlin***
```Kotlin
    fun main() {
        var user1 = Usuario(System.currentTimeMillis(), "Flávio", "flavio@outlook.com")

        // TODO: 24/07/2022 Forma simples de copiar objetos no Kotlin
        var user2 = Usuario(user1.id, user1.name, user1.email)
        println("Meu nome é: ${user2.name}, e o endereço do meu e-mail é: ${user2.email}")

        // TODO: 24/07/2022 Forma rápida de copiar todos os dados de um objeto no Kotlin
        var user3 = user1.copy() // O copy é um recurso do data class onde não está disponivel em outras classes do Kotlin
        println("Identificador do usuário:${user3.id} \n Nome: ${user3.name}, \n E-mail: ${user3.email}")

        // TODO: 24/07/2022 Outra caracteristica do copy é a possibilidade de troca de um atributo do objeto copiado
        var user4 = user1.copy(name = "Lindalva")
        println("Identificador do usuário:${user4.id} \n Nome: ${user4.name}, \n E-mail: ${user4.email}")
    }

    data class Usuario(val id: Long, var name: String, var email: String)
```

***Pares e Trios: Estruturas de Dados Simples***
```Kotlin
    fun main() {
        // TODO: 24/07/2022 O Pair permite fazer um pareamento de chave valor
        val coordinate =
            Pair(10, 20) // Primeira forma de criar um Pair(que é um data class) e permite armazenar valores diferentes
        //val coor = 10 to 20 Segunda forma de Criar um Pair
        /*
         O Pair permite trabalhar com tudo que seja com valores Duplos, eliminando a necessidade de criar um data class
         */

        // Exibir primeiro valor
        println(coordinate.first)
        // Exibir segundo valor
        println(coordinate.second)

        // TODO: 24/07/2022 Declarar valores triples
        val triple = Triple("Buíque", "Pernambuco", "Brazil")
        println("Cidade: ${triple.first} \n Estado: ${triple.second} \n ${triple.third}")
    }
```

***Herança***
```Kotlin
    fun main() {
        val p = Professor("Flávio", "Pernambuco")
        println(p.descricao())
        val a = Aluno(System.currentTimeMillis(), "Rafael", "Buíque")
        println("ID: ${a.idMatricula} \n informações: ${a.descricao()})")
    }

    // TODO: 24/07/2022 Herança | Edar Herança

    //Super Class | Classe Mâe
    open class Pessoa(var nome: String, var endereco: String) {
        // TODO: 24/07/2022 Ao iniciar a classe como open, você permite que outras classes hedem suas propriedades em outra classe, caso contrário não é possivel acessar essas propriedades!
        fun descricao() = "Meu nome é: $nome, e eu moro em $endereco "
    }

    // TODO: 24/07/2022 Ao colocar o : ele estende a classe Pessoa
    class Professor(nome: String, endereco: String) : Pessoa(nome, endereco) {

    }

    class Aluno(var idMatricula: Long, nome: String, endereco: String) : Pessoa(nome, endereco) {
        // TODO: 24/07/2022 A classe aluno extende os atributos da classe pessoa e o idMatricula é único. Pertence apenas a classe Aluno
    }
```

***Nível de Acesso***
```Kotlin
    fun main() {
        val p = Professor("Flávio", "Pernambuco")
        println(p.descricao())
        val a = Aluno(System.currentTimeMillis(), "Rafael", "Buíque")
        println("ID: ${a.idMatricula} \n informações: ${a.descricao()})")
    }

    // TODO: 24/07/2022 Herança | Edar Herança

    //Super Class | Classe Mâe
    open class Pessoa(var nome: String, var endereco: String) {
        /*
        Através do private ninguém tem acesso as variáveis de um objeto, apenas a class que tem essa  variável,
        já o protected permite que classes filhas tenham acesso a essa propriedade
         */

        // TODO: 24/07/2022 protected ou protegida
        protected var acessoBiblioteca = false
        fun descricao() = "Meu nome é: $nome, e eu moro em $endereco. Nive de acesso: $acessoBiblioteca"
    }

    class Professor(nome: String, endereco: String) : Pessoa(nome, endereco) {
        init { // Mudar nivél de acesso do professor | Alterar comportamento da classe
            acessoBiblioteca = true
        }
    }

    class Aluno(var idMatricula: Long, nome: String, endereco: String) : Pessoa(nome, endereco) {

    }
```

***Internal Classes e Módulos***
```Kotlin
    internal class Encordoamento(val numeroDeCordas: Int, val marca: String)

    // TODO: 24/07/2022 O internal pode ser acessado apenas de forma interna, ficando disponivél apenas no modulo encordoamento

    open class Instrumento(var cor: String) {

        // TODO: 24/07/2022 para acessar a classe internal é necessário colocar a instancia como privada para funcionar 
        private lateinit var encordoamento: Encordoamento

        fun console() = "O instrumento é da cor $cor e tem ${encordoamento.numeroDeCordas} cordas"

        /*
         E como não é possivel acessar a classe Encordoamento, o correto é fazer com que a super class espere as propriedades,
         para que ela crie o objeto onde a class Instrumento é a única responsável por administrar a class Encordoamento.
         De grosso modo é possivel adicionar propriedades ao objeto ao mesmo tempo que não é possivel mudar o comportamento delas
         */

        fun addEncordoamento(num: Int, marca: String){
            encordoamento = Encordoamento(num, marca)
        }

    }

    class Guitarra(cor: String) : Instrumento(cor) {
        init {
            addEncordoamento(6, "NIG")
        }
    }
    
    fun main() {
    val g = Guitarra("Vermelha")
    println(g.console())
    }
```
***Classes Abstratas***
```Kotlin
    abstract class Instrumento(var nome: String) {

        // 1. internal
        // 2. abstract (abstração) é o inverso do concreto
        // 2.1 Evitar instanciar a classe PAI(que não precisa de instância)
        // 2.2 
        // Não precisa do objeto, só precisa de classes filhas e da assinatura da classe MAE/PAI


        // A assinatura da função é a mesma (afinar) -> abstrato
        // Só que, o comportamento de afinar é diferente -> concreto
        abstract fun afinar()
    }

    class Guitarra(nome: String) : Instrumento(nome) {
        override fun afinar() {
            println("Afinação em E(Mi)")
        }
    }

    class Flauta(nome: String) : Instrumento(nome) {
        override fun afinar() {
            println("Afinação em C(Dó)")
        }
    }
    
    fun main() {
    val flauta = Flauta("Flaúta X")
    println(flauta.afinar())
    }
```
***Níveis de Abstração***
```Kotlin
    // Classe vó
    abstract class Instrumento(var nome: String) {
        abstract fun afinar()
    }

    // Classe Mâe
    abstract class InstrumentoDeCorda(nome: String, var cordas: Int) : Instrumento(nome) {
        /*
        Note que a class InstrumentoDeCorda extende dados da class Instrumento porém ela não implementou a função afinar da
        classe que ela implementou, isto porque ela não é obrigada a implementar/definir o comportamento de assinatura da
        função abstract por também ser abstract e onde a classe que vier a extender dados dessa classe irão estender a
        função afinar como no exemplo da classe Guitarra.
         */
    }

    // Classe Filha
    class Guitarra(nome: String) : InstrumentoDeCorda(nome, 6) {
        override fun afinar() {
            println("Afinação em E(Mi)")
        }
    }
```

***Funções Concretas em Classes Abstratas***
```Kotlin
    // Classe vó
    abstract class Instrumento(var nome: String) {
        abstract fun afinar()
        fun  tocar(){
            /*
            Uma classe abstrata também pode ter funções concretas
             */
            println("Tocandi a música")
        }
    }
```

***Abstract Class Bidirecional***
```Kotlin
    // Classe vó
    abstract class Instrumento(var nome: String) {

        /*
           Como deixar o código mais flexivel e generico possivel com abstract class, fazendo com que a classe
           pai/mae consiga usar o  comportamento da classe filha para fazer alguma coisa
         */
        abstract fun afinar(): Boolean

        fun tocar() {
            if (afinar()) {
                println("Tocando a música")
            } else {
                println("Afine seu instrumento")
            }
        }
    }

    // Classe Mâe
    abstract class InstrumentoDeCorda(nome: String, var cordas: Int) : Instrumento(nome) {

    }

    // Classe Filha
    class Guitarra(nome: String) : InstrumentoDeCorda(nome, 6) {
        override fun afinar(): Boolean {
            println("Afinação em E(Mi)")
            return true
        }
    }
```

***Parâmetros de Super Classes***
```Kotlin
    fun main() {
        val g = Guitarra("Tocando melodia")
        tocar(g)
    }

    fun tocar(instrumento: Instrumento) {
        instrumento.tocar()
    }
```

***Sobescrita de funções abstratas***
```Kotlin
    fun main() {
        val btn = Btn("Salvar", 340348, Pair(20, 30))
        btn.render()
    }

    abstract class Component {

        abstract fun position(): Pair<Int, Int>

        open fun render() {
            println("Desenhando a tela${position().first} | ${position().second}")
        }

    }

    abstract class Text(val text: String) : Component() {
        override fun render() {
            super.render()
            println("Desenhando o texto $text")
        }
    }

    class Btn(text: String, val backgroundColor: Int, val pos: Pair<Int, Int>) : Text(text) {
        override fun position(): Pair<Int, Int> {
            return pos
        }
    }

    class Link(text: String, val pos: Pair<Int, Int>) : Text(text) {
        override fun position(): Pair<Int, Int> {
            return pos
        }
    }
```

***Coleções de Dados Básicos***
```Kotlin
    fun main() {
        // TODO: 25/07/2022  arrayof são arrays de objetos
        val items = arrayOf(1, 2, 3, 4, 5, 6, 7)

        /*
            // TODO: 25/07/2022 intArrayOf - Lista de inteiros | Além dos inteiros existem outros tipos de arrays do tipo double, string etc
        val itemsInt = intArrayOf()
         */

        // TODO: 25/07/2022 Formas de exibir os dados que foram atribuidos dentro do array e exibilos na tela através de um for
        items.forEach {
            // TODO: 25/07/2022 forma 1
            println(it)
        }

        items.forEach { numbers ->
            // TODO: 25/07/2022 forma 2
            println(numbers)
        }

        items.forEach { println(it) }
        // TODO: 25/07/2022 forma 3 f
    }
```

***Listas de Objetos Fixos***
```Kotlin
    fun main() {
        // TODO: 25/07/2022 Para remover um usuário é necessário criar um objeto que aceite nullable
        val usuarios = arrayOf<Usuario?>( // Objeto com o tipo indefinido
            // TODO: 25/07/2022 Preenchendo o array através da classe Usuario | Coleção de tamanho fixo
            Usuario("Flávio", true),
            Usuario("Rafael", false),
            Usuario("Carol", false),
            Usuario("Isa", false),
            Usuario("Lindalva", true),
            Usuario("Amâncio", false)
        )
        usuarios.forEach { println(it) }

        // TODO: 25/07/2022 adicionar novo usuario em uma lista existente
        val addNewUsuario = usuarios.plus(Usuario("Rone", false))
        addNewUsuario.forEach { println(it) }

        // TODO: 25/07/2022 Para buscar um elemento da lista é através de indices onde o primeiro item da lista começa como zero
        println("Exibindo primeiro item da lista ${usuarios[0]}")

        // TODO: 25/07/2022 Atualizar um item da lista
        usuarios[2] = Usuario("Amanda", false)
        println(usuarios[2])

        // TODO: 25/07/2022 Removendo usuario
        usuarios[0] = null
        usuarios.forEach { println(it) }
    }

    data class Usuario(var name: String, var isAdmin: Boolean)
```

# REGRAS DE NOMEAÇÃO E ESCRITA NO KOTLIN

> ***CAMEL CASE - É uma regra aplica em variáveis por palavras compostas ou frases, onde cada palavra é iniciada com maiúsculas e unidas sem espaços, excerto a primeira letra depois de da variável {voceTemQueEscreverDessaManeira}*** 

> ***Variáveis sempre devem começar com letra minúscula***

> ***Não é utilizado no Koltin caracteres especiais***

> ***Funções não podem conter o mesmo nome***

> ***Nome de classes começam a primeira letra maiúscula***
