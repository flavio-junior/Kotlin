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

# REGRAS DE NOMEAÇÃO E ESCRITA NO KOTLIN

> ***CAMEL CASE - É uma regra aplica em variáveis por palavras compostas ou frases, onde cada palavra é iniciada com maiúsculas e unidas sem espaços, excerto a primeira letra depois de da variável {voceTemQueEscreverDessaManeira}*** 

> ***Variáveis sempre devem começar com letra minúscula***

