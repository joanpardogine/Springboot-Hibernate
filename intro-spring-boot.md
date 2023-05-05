<!-- https://cursos.arquitecturajava.com/courses/521050/lectures/9531679 -->


# Introducción a Spring Boot

Spring Boot és un Framework que simplifica el desvolupament de Spring.

## Maven y Spring

![intro-spring-boot-0001.png](./imatges/intro-spring-boot-0001.png)


Amb un entorn sense **Spring**, el que normalment es fa, és des de una **Classe** **```Main```**, es crida al constructor de la **Classe** **```Main```**, i normalment fent un **```new```**, i aquesta ens instanciarà l'objecte com un **``servei``**, i ja està, no cal fer res més per poder treballar amb el **```Servei```** sense més.


![intro-spring-boot-0002.png](./imatges/intro-spring-boot-0002.png)

Mentre que amb un entorn amb **Spring**, és **Spring** qui instancia el **```Servei```**, i instancía el **```Servei```** amb el seu **``context``**. I una vegada fet això, ja podem fer servir el **Servei**, sense cap problema. Quan es fa servir aquesta metodologia, es diu que s'ha fet una **Injecció de dependència**.

![intro-spring-boot-0003.png](./imatges/intro-spring-boot-0003.png)

Pero realment, que és el que està pasant.

Aquí veiem TOTS els passos que cal fer:

![intro-spring-boot-0004.png](./imatges/intro-spring-boot-0004.png)


1. Instal·lar les dependències Spring
1. Crear el fitxers de @configuration
1. *Crear el programa **```main```***
1. Inicialitzar el **```context```**, és el fitxer que ens indica quins son els **Bean**s
1. Registrar el fitxer de configuració
1. Obtenir el **``Bean``**`
1. ***Invocar-lo***


Aparentment, podriem pensar que hauria de ser tan fàcil com simplement fer els pasos 3 i 5. Pero en realitat no és així.

Començarem creant el projecte **```Hello World```**, com de costum i aixi veurem tots els pasos.

## Creació del projecte **```Hello World```**

### Com funciona **```Spring```**
Caldra fer el següent:

Crearem un Servei i aquest Servei estarà registrat a través d'un configurador.
Aquest configurador caldrà que faci un **```Component Scan```**, per indicar quines Classes i a quins Paquets registrarà Serveis.

En aquest cas, només caldrà que registri/inicialitzi solament el nostre **```Servei```**, el **``Main``**.

![intro-spring-boot-0005.png](./imatges/intro-spring-boot-0005.png)


En resum, **Spring** el que farà serà **carregar** el **```Context```**, el **```Context```** **instanciarà** el **```Servei```**, i des del **```Main```**, ja podrem fer servir el nostre **```Servei```**, i això ho farem **invocant** aquest **```Servei```**, **registrat** des del **Framework Spring**, des del nostre programa.

![intro-spring-boot-0006.png](./imatges/intro-spring-boot-0006.png)

### Creació del projecte **```Hello World```**

1. Descarregar JDK
2. Instal·lar IDE (IntelliJ IDEA)

## Ejemplo de Maven y Spring

![intro-spring-boot-0007.png](./imatges/intro-spring-boot-0007.png)

![intro-spring-boot-0008.png](./imatges/intro-spring-boot-0008.png)

New Project

Name: HelloWorld
Loacation: C:\00-proj-java\HelloWorld
Language: Java
Build system: Maven
JDK: 17

GroupID: com.projectes
ArtifactId: springframework1


![intro-spring-boot-0009.png](./imatges/intro-spring-boot-0009.png)

![intro-spring-boot-0010.png](./imatges/intro-spring-boot-0010.png)

![intro-spring-boot-0011.png](./imatges/intro-spring-boot-0011.png)


> Microsoft Defender configuration
> The IDE has detected Microsoft Defender with Real-Time Protection enabled. It might severely degrade IDE performance. It is recommended to add following paths to the Defender folder exclusion list:    C:\00-proj-java\HelloWorld\HelloWorld   C:\Users\???\AppData\Local\JetBrains\IdeaIC2023.1  Choose "Automatically" to run a script that excludes these paths (note: Windows will ask for administrative privileges). Choose "Manually" to see Defender configuration instructions.

![intro-spring-boot-0013.png](./imatges/intro-spring-boot-0013.png)


> Microsoft Defender configuration
> Microsoft Defender configuration script failed. Please look for "WindowsDefenderChecker" records in the log.

![intro-spring-boot-0014.png](./imatges/intro-spring-boot-0014.png)


1. Obrim el **```pom.xml```** que és el fitxer a on cal configurar les dependencies.

I afegim les següents línies:

```
    <build>
        <plugins>
            <plugin>
                <groupId>org.apache.maven.plugins</groupId>
                <artifactId>maven-compiler-plugin</artifactId>
                <version>3.8.0</version>
                <configuration>
                    <source>1.8</source>
                    <target>1.8</target>
                </configuration>
            </plugin>
        </plugins>
    </build>
```

Anem al [repositori de Maven](https://mvnrepository.com/)

I busquem algunes dependencies que farem servir:

### **1.** [Spring core](https://mvnrepository.com/search?q=spring+core)

![intro-spring-boot-0016.png](./imatges/intro-spring-boot-0016.png)

### **1.** [Spring core](https://mvnrepository.com/search?q=spring+core)

![intro-spring-boot-0016.png](./imatges/intro-spring-boot-0016.png)

![intro-spring-boot-0017.png](./imatges/intro-spring-boot-0017.png)

![intro-spring-boot-0018.png](./imatges/intro-spring-boot-0018.png)

```xml
<!-- https://mvnrepository.com/artifact/org.springframework/spring-core -->
<dependency>
    <groupId>org.springframework</groupId>
    <artifactId>spring-core</artifactId>
    <version>6.0.8</version>
</dependency>
```


### **2.** [Spring context](https://mvnrepository.com/search?q=spring+context)

![intro-spring-boot-0019.png](./imatges/intro-spring-boot-0019.png)

![intro-spring-boot-0020.png](./imatges/intro-spring-boot-0020.png)

![intro-spring-boot-0021.png](./imatges/intro-spring-boot-0021.png)

```xml
<!-- https://mvnrepository.com/artifact/org.springframework/spring-context -->
<dependency>
    <groupId>org.springframework</groupId>
    <artifactId>spring-context</artifactId>
    <version>6.0.8</version>
</dependency>
```

Quedant de la següent manera:

![intro-spring-boot-0022.png](./imatges/intro-spring-boot-0022.png)

Fins aquí el que acavem de fer, és configurar el nostre projecte perque funcioni amb **```springframework```**, i tot i que pot semblar fàcil, com sempre, cal saber que s'ha de fer i com fer-ho!

 Com es pot veure, hi ha **```errors```** o **```warnings```**, això és perque no està actuialitzat el projecte, per refrescar el preojecte cal:

 1. Obrir la secció de **Build**:

![intro-spring-boot-0023.png](./imatges/intro-spring-boot-0023.png)

 I pressione la icona de **```refresh```**!

![intro-spring-boot-0024.png](./imatges/intro-spring-boot-0024.png)

I quan acabi de refrescar el projecte, ja no han d'apareixer ni **```errors```** ni **```warnings```**!


![intro-spring-boot-0025.png](./imatges/intro-spring-boot-0025.png)


![intro-spring-boot-0026.png](./imatges/intro-spring-boot-0026.png)

New Package: com.HelloWorld.serveis

![intro-spring-boot-0027.png](./imatges/intro-spring-boot-0027.png)

![intro-spring-boot-0028.png](./imatges/intro-spring-boot-0028.png)


Servei

![intro-spring-boot-0029.png](./imatges/intro-spring-boot-0029.png)

Per defecte ja ens ha creat el fitxer i la classe:

```java
package com.HelloWorld.serveis;

public class Servei {
    }
```

I ara anem a crear el que nosaltres volem, és a dir un mètode anomenat **```missatge```** que mostri el missatge **```Hola món!```**:

```java
package com.HelloWorld.serveis;

public class Servei {
    public void missatge(){
        System.out.print("Hola món!");
    }
}
```

I ara com a cosa especifica de **```Spring```**, cal que fem servir les etiquetes d'**```Spring```**, per tatn cal afegir **```@Service```**, per indicar-li que es tracta d'un servei.

```java
package com.HelloWorld.serveis;

@Service
public class Servei {
    public void missatge(){
        System.out.print("Hola món!");
    }
}
```

![intro-spring-boot-0031.png](./imatges/intro-spring-boot-0031.png)

```java
package com.HelloWorld.serveis;

import org.springframework.stereotype.Service;

@Service
public class Servei {
    public void missatge(){
        System.out.print("Hola món!");
    }
}
```

Com ja hem comentat abans ara cal crear el fitxer de configuració.

![intro-spring-boot-0032.png](./imatges/intro-spring-boot-0032.png)


SpringConfigurador

![intro-spring-boot-0033.png](./imatges/intro-spring-boot-0033.png)


```java
package com.HelloWorld.serveis;

import org.springframework.context.annotation.ComponentScan;
import org.springframework.context.annotation.Configuration;

@Configuration
@ComponentScan("com.HelloWorld.serveis")
public class SpringConfigurador {
    }

```

Ara ja només ens queda crear un programa **```main```** que ens faci una instancia del Servei a traves de framework Spring i en mostri el missatge per pantalla.


![intro-spring-boot-0038.png](./imatges/intro-spring-boot-0038.png)


SpringMain

![intro-spring-boot-0039.png](./imatges/intro-spring-boot-0039.png)

Cal recordar que Spring Boot es bassa en anotacions (Annotations).

