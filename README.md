# Kotlin-Java Interop

This is a minimal project that demonstrates Kotlin/Java interop in the Cursor IDE.

## Project Structure
- Kotlin 2.0
- Java 21
- Maven
- A `Calculator.kt` that is meant to be called from Java main defined in `JavaMain.java` and a Kotlin main defined in `KotlinMain.kt`

## In the Terminal

This command shows that you can call Kotlin from Java at runtime without issues ...

```
mvn clean compile exec:java -Dexec.mainClass=com.example.JavaMain
```

This command shows that you can call Kotlin from Kotlin at runtime without issues ...

```
mvn clean compile exec:java -Dexec.mainClass=com.example.KotlinMainKt
```

## The Problem

Open `JavaMain.java`, in the Problems tab you will see `The import com.example.Calculator cannot be resolved`.  I have tried the following extension combinations.  All exhibit the same behavior ...
- Java + Kotlin(daplf) 
- Kotlin(fwcd) and Java w/ Language Support for Java
- Kotlin Language(mathiasfrohlich) and Java w/ Language Support for Java