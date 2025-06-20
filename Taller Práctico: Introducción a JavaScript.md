Taller-Práctico-Introducción-a-JavaScript


## Parte 1: Explorando JavaScript

### 1.1 Explica con tus palabras qué es JavaScript y en qué se diferencia de HTML y CSS.
    


```
    R:// Javascript es un lenguaje de programación que es muy usado, por ahí escuché que el 98% de las páginas que hay en internet usan JS
         tengo entendido que los anvegadores en si son un "interprete" de javascript, entonces eso lo hace muy útil.
         Sirve para darle funcionalidad a los elementos estáticos de las páginas web, como hacer una galería, o hacer que los elementos cambien cuando pasen cosas.
         En css el ::hover da cierta funcionalidad o interactividad, pero eso es muy suave con respecto a lo que se puede hacer con JS  
 ```  

#### 1.2 Enumera al menos tres características principales de JavaScript.

    Es un lenguaje de alto nivel, interpretado y oriendato a objetos
    Inicialmente llamado Mocha, luego LiveScript, finalmente se conoció como JavaScript

### 1.3 ¿Qué significa que JavaScript sea un lenguaje "interpretado" y "basado en eventos"?

```  
    Que sea interpretado implica que es un lenguaje que se va interpretando linea por linea, es decir de haber un error, el error surgiría en el momento que se use esa linea de código donde está el error
    mientrastanto, un lenguaje compilado tiraría el error inmediatamente se trata de usar. el hecho de que sea interpretado lo hace más dinámico, y cuando son compilados, generalmente tienen mejor rendimiento.
 ```  
## Parte 2: Variables y Tipos de Datos

### 2.1 Declara una variable nombre y asígnale tu nombre. Luego, muestra un saludo en la consola que diga "Hola, [nombre]".
    
    let nombre = "felipe";
    console.log(nombre)
    
            
### 2.2 Crea tres variables: una con un número entero, otra con un número decimal y otra con una cadena de texto. Muestra cada una en la consola usando console.log().
        
       
        let nombre = "felipe";
        let edad = 25;
        let peso = 90.3;
        console.log(`Mi nombre es ${nombre} tengo ${edad} años y peso ${peso} kilos`); 
       
    
### 2.3 Declara una constante llamada PI con el valor 3.1416. Intenta cambiar su valor y observa qué sucede.
    
    const PI = 3.1416;

    PI = 15;
    
### 2.4 Declara una variable sin asignarle valor. Muestra en consola qué contiene.



![imagen](https://github.com/user-attachments/assets/fd11d936-92b8-4c68-b618-66e2e44fd684)

    
### 2.5 Crea una variable con valor null y otra con un valor booleano. Muestra ambos en consola.



![imagen](https://github.com/user-attachments/assets/9f081330-5496-4db0-aaf0-04226caf65e6)

    
## Parte 3: Entrada y Salida de Datos

3.1 Usa prompt() para pedirle al usuario su edad y guárdala en una variable. Luego, muestra en consola un mensaje que diga "Tienes [edad] años".

![imagen](https://github.com/user-attachments/assets/43de1383-f433-49c3-9034-b6ecaf8d9175) 




(no leí bien ._.)




![imagen](https://github.com/user-attachments/assets/692000c4-6af8-4fab-b66e-dbb100c11f9e)



3.2 Usa alert() para mostrar un mensaje de bienvenida.


![imagen](https://github.com/user-attachments/assets/3826b903-d6f5-480d-866f-4ea570a601a0)



3.3 Usa confirm() para preguntar al usuario si desea continuar. Muestra en consola el valor que devuelve esta función.


![imagen](https://github.com/user-attachments/assets/5c61ba50-68a7-4c89-bd67-b9fb1e775642)

Parte 4: Operadores


4.1 Declara dos variables numéricas. Realiza y muestra los resultados de las siguientes operaciones: suma, resta, multiplicación, división y módulo.

![imagen](https://github.com/user-attachments/assets/3a98c20c-57b5-4ba6-ae26-faaf9e3acf91)


4.2 Declara dos variables con cadenas de texto y únelas en una nueva variable usando el operador de concatenación.

![imagen](https://github.com/user-attachments/assets/fd1a6708-107d-44c6-90ae-a764053983f7)

4.3 Evalúa y muestra en consola el resultado de las siguientes comparaciones:
![image](https://github.com/user-attachments/assets/2671fa5c-3fa6-4bda-8804-97b1bbf3e456)


Parte 5: Condicionales

// 5.1 Crea un programa que pida al usuario un número y muestre en consola si es mayor, menor o igual a 10.
    
    let num = prompt("por favor ingrese un número")
    
     if (num > 10) {
        console.log("el número que ingresó es mayor a 0")} 
    else if (num < 10){
        console.log("el número que ingresó es menor que 10")
    }
        else {    
            console.log("el número es igual a 10")
        }




5.2 Crea un programa que solicite el nombre de un usuario y compare si se llama "Admin". Si es así, muestra un mensaje de bienvenida especial, de lo contrario, un mensaje genérico.



    let nombre = prompt("por favor identificaté").trim()
    
    if (nombre == "admin"){
        console.log("Bienvenido señor admin <3")
    }
    else {
        console.log(`lo siento ${nombre} no tengo idea de quien eres`);

5.3 Usa el operador ternario para mostrar si un número ingresado es par o impar.

// 5.3 Usa el operador ternario para mostrar si un número ingresado es par o impar.
    
    let numo = prompt("ingrese un núḿero porfavor")
    
    numo % 2 == 0 ? console.log(`El número ${numo} es par`) : console.log(`El número ${numo} es impar`);

Parte 6: Consola del Navegador

6.1 Muestra diferentes tipos de mensajes en la consola:

    Un mensaje informativo (console.info)
        ```
            let edad = prompt("Cual es tu edad?")
    if (edad<18){
        console.info(`el usuario tiene ${edad} años, algunas funciones deberían de estar restringidas`);
    }
    else {console.info(`el usurio tiene ${edad} tiene total acceso al contenido`)
    }  
        ```
Un mensaje de advertencia (console.warn)
        ![imagen](https://github.com/user-attachments/assets/16e24ba2-2c1a-4940-8325-84e5e2df6ed5)
            
            let acceso = prompt("Tiene permiso para accedera esta zona (y/n)").trim().toLowerCase();
        if (acceso == "y"){
            console.info("Bienvenido jefe");
        }
        else {
            console.warn("por abstengase de ingresar")
        }

Un mensaje de error (console.error)
![imagen](https://github.com/user-attachments/assets/52c483a4-d622-433f-a74d-97614abb7c63)

    let asistencia = prompt("escriba la hora de entrada (sólo el número)");
            if (asistencia <= 6){
                console.log("llegó a tiempo")
            }
            else{ console.error("llegaste tarde")}

   

Un grupo de mensajes (console.group y console.groupEnd)
![imagen](https://github.com/user-attachments/assets/d2eb2d75-c65d-4a54-ba18-ca302b2e2b37)

        console.groupconsole.group("Trabajenguas en español");
    console.info("Pablito clavó un clavito. ¿Qué clavito clavó Pablito?");
    console.info("Tres tristes tigres tragaban trigo en un trigal.");
    console.info("El cielo está enladrillado. ¿Quién lo desenladrillará? El que lo desenladrille, buen desenladrillador será?");
    console.info("PPepe Pecas pica papas con un pico. ¿Con qué pico pica papas Pepe Pecas");
    console.groupEnd();
    
El tiempo que tarda un bloque de código en ejecutarse (console.time y console.timeEnd)

![imagen](https://github.com/user-attachments/assets/66a5892b-2f9d-4a99-8f89-7c7cf946c8df)

        console.time("OperacionPesada"); 
    
    for (let i = 0; i < 1000000; i++) {
      console.log(` el valor de i es ${i}`);
    }
    
    
    console.timeEnd("OperacionPesada");
    
    console.log("Simulación finalizada.");

Parte 7: Comentarios

7.1 Escribe un pequeño bloque de código donde utilices comentarios de una línea y de varias líneas para explicar lo que hace cada parte.

        //     El tiempo que tarda un bloque de código en ejecutarse (console.time y console.timeEnd)
    
    console.time("OperacionPesada");  //ponemos el nombre a al cronometro
    
    for (let i = 0; i < 1000000; i++) {
      console.log(` el valor de i es ${i}`); //una operación larga que demanda computo
    }
    
    console.timeEnd("OperacionPesada"); //no muestra el valor del crónometro
    
    console.log("Simulación finalizada.");

Parte 8: Desafío Final

8.1 Crea un archivo HTML y vincúlalo con un archivo .js externo. En ese archivo:
![imagen](https://github.com/user-attachments/assets/200aadbc-900d-4897-a0eb-43c4451b7186)

![imagen](https://github.com/user-attachments/assets/d853764c-3774-46f6-9526-8684516d92a2)

