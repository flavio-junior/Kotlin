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

# REGRAS DE NOMEAÇÃO E ESCRITA NO KOTLIN

> ***CAMEL CASE - É uma regra aplica em variáveis por palavras compostas ou frases, onde cada palavra é iniciada com maiúsculas e unidas sem espaços, excerto a primeira letra depois de da variável {voceTemQueEscreverDessaManeira}*** 

> ***Variáveis sempre devem começar com letra minúscula***

