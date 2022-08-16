
<hr>
<meta charset="UTF-8">
Desafíos:

<br>1. Crea una función de lotería que reciba un número n y sortee un número entre 0 a n, retornando ese valor. 
<br>De esta forma, en vez de escribir var numeroPensado = Math.round(Math.random()*n);, escribirás var 
<br>numeroPensado = sortea(n);. Realiza esa modificación, creando una nueva función y utilízala de forma correcta.
<br>2. Hacer que tu juego exhiba, cuando el usuario falle el intento, si el número lanzado era mayor o menor al 
<br>número pensando por el programa.

<h1>PROGRAMA JUEGO DE ADIVINACION </h1>


<script>

    function saltarLinea() {
        document.write("<br>");    
        document.write("<br>");    
        document.write("<br>");    
    }  

    function imprimir(frase) {
        document.write(frase);
        saltarLinea();
    }
      function sorteo(n) {
        return Math.round(Math.random()*10);
    
    }
     var numeroPensado = sorteo(10)
     var numeroLanzado = parseInt(prompt("Ingrese un número"))

    if (numeroPensado == numeroLanzado){
        imprimir("usted acertó")
    }

    else {
        if(numeroPensado > sorteo(10)) {
        imprimir("Usted erró, el numero Era menor")
        }
        
        else{
        imprimir("Usted erró, el numero era mayor")
        }
    }
        

</script>
<br>
<br>

<meta charset="UTF-8">

<script>
    function saltarLinea() {
        document.write("<br>");
    }

    function imprimir(frase) {
        document.write(frase);
        saltarLinea();
    }

    var edad = parseInt(prompt("¿Cuál es tu edad?"));
    var tieneLicencia = prompt("¿Tienes licencia? Responde S o N");

    if((edad >= 18) && (tieneLicencia == "S")) {
            imprimir("Puedes conducir");
        }

    else {
        imprimir("No puedes conducir");
    }

</script>




<meta charset="UTF-8">

<script>
    //RESPUESTA DEL MAESTR= ERRADA YA QUE SI ES MAYOR DE EDAD Y NO TIENE LICENCIA NO APARECE NADA.
    function saltarLinea() {
        document.write("<br>");
    }

    function imprimir(frase) {
        document.write(frase);
        saltarLinea();
    }

    var edad = parseInt(prompt("¿Cuál es tu edad?"));
    var tieneLicencia = prompt("¿Tienes licencia? Responde S o N");

    if((edad >= 18) && (tieneLicencia == "S")) {
            imprimir("Puedes conducir");
        }


    if(edad < 18) {
        imprimir("No puedes conducir");
    }

</script>







<meta charset="UTF-8">

<script>
    //RESPUESTA DEL MAESTR= ERRADA YA QUE SI ES MAYOR DE EDAD Y NO TIENE LICENCIA NO APARECE NADA.
    function saltarLinea() {
        document.write("<br>");
    }

    function imprimir(frase) {
        document.write(frase);
        saltarLinea();
    }

    var edad = parseInt(prompt("¿Cuál es tu edad?"));
    var tieneLicencia = prompt("¿Tienes licencia? Responde S o N");

    if(edad >= 18) {
        if(tieneLicencia == "S") {
            imprimir("Puedes conducir");
        }
    }

    if(edad < 18) {
        imprimir("No puedes conducir");
    }

</script>


<hr>

<br> 

<meta charset="UTP-8">
<H1> PROGRAMA QUE CALCULA LOS PUNTOS DE UN EQUIPO DE FUTBOL</H1>
<script>
function saltarLinea() {
    document.write("<br>");
    document.write("<br>")

}

function imprimir(frase) {
    document.write(frase);
    saltarLinea();


}

    var victorias = parseInt (prompt("Informe la cantidad de Victorias"));
    var empates = parseInt(prompt("Informe la cantidad de Empates"));
    var puntostotal = (victorias * 3) + empates;
    imprimir("El total de puntos del equipo es: " + puntostotal);

    


</script>
<br>
<meta charset="UTF-8">
<h1><big>PROGRAMA IMC</big></h1>
<br>
<script>
    //IMC=Indice de masa corporal
    function saltarLinea() {
        document.write("<br>");    
        document.write("<br>");    
       
            
    }  
    function imprimir(frase) {
        
        document.write ("<big>" + (frase) + "</big>");
        saltarLinea();
    
    }
    function calcularImc(peso,altura,nombre) {
        imc = peso / (altura * altura);
        imprimir(nombreInformado + ", su IMC calculado es: " + imc)
        return(imc);
    }
    nombreInformado= prompt("Informe su nombre ")
    pesoInformado= prompt("Informe su peso ")
    alturaInformado= prompt("Informe su altura ")
    imcInformado= calcularImc(pesoInformado,alturaInformado)
    







</script>
      <hr>  


<br> // CODIGO QUE MUESTRA LA SUMA DE DOS NUMEROS a Y b, DONDE SE EJECUTAN DESDE UNA FUNCION CON EL USO DEL RETORNO
<br> ENTONCES FUNCION A + FUNCION B RESULTA:
<br><br><meta charset="UTF-8">

<script>
    function saltarLinea() {

        document.write("<br>");
    }

    function mostrar(frase) {
        document.write(frase);
        saltarLinea();
    }

    function a(numero1, numero2) {
        return numero1 + numero2;
    }

    function b(numero1, numero2) {
        return numero1 / numero2;
    }

    var resultado = a(10,20) + b(30,2);

    mostrar(resultado);
</script>
<br>
<hr>
<br>
<br> AUN MAS EFICIENTE QUE EL ANTERIOR IMC
<br>
<meta charset="UTF-8">
<h1><big>PROGRAMA IMC</big></h1>
<br>
<script>
    //IMC=Indice de masa corporal
    function saltarLinea() {
        document.write("<br>");    
        document.write("<br>");    
       
            
    }  
    function imprimir(frase) {
        
        document.write ("<big>" + (frase) + "</big>");
        saltarLinea();
    
    }
    function calcularImc(peso,altura,nombre) {
        imc = peso / (altura * altura);
        imprimir("El IMC calculado es: " + imc)
        return(imc);
        

    }   
   
    //importante que las variables al momento de declararla y de llamarlas tengas las mayúsculas y las minusculas igual escritas
    

    imcChristian= calcularImc(71,1.72, "Christian");
    imcChristian= calcularImc(75,1.73,"Felipe");

        
   
</script>
<br>
<hr>
<hr>
<br>
<hr> MAS EFICIENTE QUE EL ANTERIOR IMC
<br>
<meta charset="UTF-8">
<h1><big>PROGRAMA IMC</big></h1>
<br>
<script>
    //IMC=Indice de masa corporal
    function saltarLinea() {
        document.write("<br>");    
        document.write("<br>");    
       
            
    }  
    function imprimir(frase) {
        
        document.write ("<big>" + (frase) + "</big>");
        saltarLinea();
    
    }
    function calcularImc(peso,altura) {
        imc = peso / (altura * altura);
        imprimir("El IMC calculado es: " + imc)
        return(imc);
        

    }   
   
    //importante que las variables al momento de declararla y de llamarlas tengas las mayúsculas y las minusculas igual escritas
    

    imcChristian= calcularImc(71,1.72);
    imcChristian= calcularImc(75,1.73);

        
   
</script>
<br>
<hr>
<hr>
<br>
<br>
<meta charset="UTF-8">
<h1><big>PROGRAMA IMC</big></h1>
<br>
<script>
    //IMC=Indice de masa corporal
    function saltarLinea() {
        document.write("<br>");    
        document.write("<br>");    
       
            
    }  
    function imprimir(frase) {
        
        document.write ("<big>" + (frase) + "</big>");
        saltarLinea();
    
    }
    function calcularImc(peso,altura) {
        imc = peso / (altura * altura)
        return(imc);
        

    }   
   
    //importante que las variables al momento de declararla y de llamarlas tengas las mayúsculas y las minusculas igual escritas
    
    pesoChristian=59
    AlturaChristian=1.56
    //imcChristian= pesoChristian / (AlturaChristian * AlturaChristian)
    imcChristian= calcularImc(pesoChristian,AlturaChristian)
    imprimir("El IMC de Christian es: " + imcChristian)

    PesoLiz=40
    AlturaLiz=1.40
    //imcLiz= PesoLiz / (AlturaLiz * AlturaLiz)
    imcLiz= calcularImc(PesoLiz, AlturaLiz)
    imprimir("El IMC de Liz es: " + imcLiz )
    
    
   
</script>
<br>
<hr>
<hr>
<br>
SOLUCION IMPRIMIR EDADES
<br>
<br>
<meta charset="UTF-8"

<br>Hagamos algunos ajustes basados en el código anterior.
<br>1.- ¡Altera la función saltarLinea para que salte cinco líneas! Es decir, hacer cinco < b r>s.
<br>2.- Realiza una etiqueta HTML, será bastante útil para separar un resultado de otro:< h r>. Altera
<br> la función saltarLinea() para que esta escriba en el navegador un < h r> después del tercer < b r> que ya hicimos.
<br>3.- La fuente de nuestro programa puede que aún no sea la adecuada. Hay una etiqueta HTML que se llama < b i g >. 
<br> Haz que la función imprimir coloque la frase entre < b i g > y </ b i g >.
<br>4.- ¿Qué pasa si te olvidas la palabra function a la hora de declarar una de las funciones? 
<br>¿Y los paréntesis en la declaración de la función saltarLinea?
<br>
<br>    
<h1>PROGRAMA</h1>
<script>
    //RTA4) Simplemente no funciona el codigo si olvidamos alguna de las dos cosas (fuction o ())
    function saltarLinea() {
        document.write("<br>");    
        document.write("<br>");    
        document.write("<br>");
        document.write("<hr></hr>")
        document.write("<br>");
        document.write("<br>");
            
    }  
    function imprimir(frase) {
        
        document.write ("<big>" + (frase) + "</big>")
        saltarLinea();
    }
    var anho = 2025;
    imprimir("hola amigos");
    // este código calcula las edades de Juan, Pedro y Carlos
    imprimir("Juan tiene: " + (anho-2000) + " años");
    imprimir("Pedro tiene: " + (anho-1995) + " años");
    anho = 2030
    imprimir("Carlos tiene: " + (anho-2005) + " años");
</script>
<br>
<br>__________________________________________________________________________________________________________________________________________
<br>
<br> SOLUCION MAESTRO
<br>
<br>
<meta charset="UTF-8">
<script>
    function saltarLinea() {
        document.write("<br>");
    }

    function imprimir(frase) {
        document.write(frase);
    }

    var miEdad = 18;
    var edadHermano = 15;

    imprimir("Nuestra diferencia de edad es " + (miEdad - edadHermano));
 </script>
<br>
<br>
<br>__________________________________________________________________________________________________________________________________________
<br>
<br>
<br>¿Cuántos años de diferencia tienes con tu hermano? 
<br>Escribe un programa que muestre el mensaje ¨Nuestra diferencia de edad es¨,
<br>concatenando el resultado de la diferencia de tu edad con la de tu hermano 
<br>(o de un amigo). La respuesta puede dar negativa, sin duda. No olvides de usar
<br>las funciones saltarLinea e imprimir y de incluir la etiqueta <meta> para 
<br>resolver problemas de acentuación. No necesitas enviar la respuesta, solo basta 
<br>crear un programa, probar y verificar si todo funciona. ¡Si tienes alguna duda no
<br>dejes de postearla en el foro!
<br>
<br>
<br><h3> Años de diferencia </h3>
<script>

    function saltarlinea() {

        document.write("<br>");
        document.write("<br>");
    }
    
    function imprimir(frase) {

        document.write(frase);
        saltarlinea();

    }


    imprimir("Mi edad es "+ (MiEdad=26));
    imprimir ("La edad de mi hermano es " + (EdadDeX=18)); 
    imprimir("Nuestra diferencia de edad es " + (resultado= MiEdad - EdadDeX));



</script>
<br>
<br>
__________________________________________________________________________________________________________________________________________
__________________________________________________________________________________________________________________________________________   
    <br>        //poderosa funcion creada: MostrarAlerta que, gracias a la función: funtion funciona :V
    <br>    // veo que se le puede indicar a la funcion creada qué clase de contenido tendra ej: frase, mensaje.

    TERCERA FUNCION: CREAR ALERTA

    <br>
    <br><meta charset="UTF-8">
    <script>
        //poderosa funcion creada: MostrarAlerta que, gracias a la función: funtion funciona :V
        // veo que se le puede indicar a la funcion creada qué clase de contenido tendra ej: frase, mensaje.


        function mostraralerta(mensaje) {

            alert("***" + mensaje + "***")
        }


        //codigo que crea alerta con sumatoria de edades
        var edad1 = 10;
        var edad2 = 20;
        var edad3 = 30;
        var totalEdades = edad1 + edad2 + edad3;
        var promedioEdades = totalEdades/3;
 
        mostraralerta("Total de edades es " + totalEdades);
        mostraralerta("La media de las edades es " +  promedioEdades);
    </script>
   
   <br>
   <br>
   __________________________________________________________________________________________________________________________________________
   <br><meta charset="UTF-8">
   <br> 
   <br>Juana tiene la costumbre de colocar siempre tres asteriscos antes y después de los mensajes de advertencia. 
   <br>
   <br>Veamos un ejemplo de su código:
   <br>
   <script>
       var edad1 = 10;
       var edad2 = 20;
       var edad3 = 30;
       var totalEdades = edad1 + edad2 + edad3;
       var promedioEdades = totalEdades/3;
       alert("***Total de edades es " + totalEdades + "***");
       alert("***La media de las edades es " +  promedioEdades + "***");
   </script>
   <br>
   <br>

__________________________________________________________________________________________________________________________________________
    <br>
    <br><meta charset="UTP-8">
    <br><h3>FUNCIONES</h3>
    
<script>
    
    
    function saltarlinea() {
        document.write("<br>");
    }
  

    function imprimir(frase) {

        document.write(frase);
        saltarlinea();
    }   

      
    saltarlinea();
    imprimir("Mi primera funcion es saltar línea")
    saltarlinea();

    //importante que la variable tuve que declarla a esta altura porque al principio no me la permitió
    //importante debo aplicar llamar funciones dentro de funciones
    anho=2025   
    imprimir("Pedro tiene " + (anho-1996) + " años");
    saltarlinea();
    imprimir("mi segunda funcion es imprimir con concatenar");
</script>
    <br>
    <br>
    <br>
__________________________________________________________________________________________________________________________________________
        <br><meta charset="UTF-8">
        <h3>¿Alcohol o Gasolina?</h3>
    
    <script> 
         var tanque = 40;
    
        var caminoConGasolina = 480;
        var consumoDeGasolina = caminoConGasolina/tanque;
        var caminoConAlcohol = 300;
        var consumoDeAlcohol = caminoConAlcohol/tanque;
    
        document.write("La eficiencia del carro usando gasolina es " + consumoDeGasolina + " km/L"); 
        document.write("<br>"); 
        document.write("La eficiencia del carro usando alcohol es " + consumoDeAlcohol + " km/L");
    
    </script>
    <br>
    <br>
    <br>__________________________________________________________________________________________________________________________________________
    <br>
    FACILITANDO NUESTRAS VIDAS- OPINION INSTRUCTOR
    <br>
    <meta charset="UTF-8">
    <script>
        var tablaDeMultiplicar = 8;
        document.write(tablaDeMultiplicar + " veces 1 es " + tablaDeMultiplicar* 1 + "<br>");
        document.write(tablaDeMultiplicar + " veces 2 es " + tablaDeMultiplicar* 2 + "<br>");
        document.write(tablaDeMultiplicar + " veces 3 es " + tablaDeMultiplicar* 3 + "<br>");
        document.write(tablaDeMultiplicar + " veces 4 es " + tablaDeMultiplicar* 4 + "<br>");
        document.write(tablaDeMultiplicar + " veces 5 es " + tablaDeMultiplicar* 5 + "<br>");
        document.write(tablaDeMultiplicar + " veces 6 es " + tablaDeMultiplicar* 6 + "<br>");
        document.write(tablaDeMultiplicar + " veces 7 es " + tablaDeMultiplicar* 7 + "<br>");
        document.write(tablaDeMultiplicar + " veces 8 es " + tablaDeMultiplicar* 8 + "<br>");
        document.write(tablaDeMultiplicar + " veces 9 es " + tablaDeMultiplicar* 9 + "<br>");
        document.write(tablaDeMultiplicar + " veces 10 es " + tablaDeMultiplicar* 10 + "<br>");
    </script>
    <br>
    <br>
    <br>
    
__________________________________________________________________________________________________________________________________________
    <br>
    FACILITANDO NUESTRAS VIDAS - INTENTO UNO FALLIDO
    <br>
    //Quise usar álgebra en vez de planas pero debo conceptualizar primero//
    <br>
    <br>
__________________________________________________________________________________________________________________________________________
    <br>
    FACILITANDO NUESTRAS VIDAS- INTENTO DOS FALLIDO
    <br>
    //Quise usar álgebra en vez de planas pero ya no entiendo nada y debo dormir 4:00am
    //Clase a las 7:00 de Examen//
__________________________________________________________________________________________________________________________________________

<br>
<script>
    

    a=8
    b=3
    c=a*b
    document.write<br>
    document.write(a*b)
    document.write<br>
    
</script>

    <br>
    <br>
__________________________________________________________________________________________________________________________________________
    <br>
    <br>
    ¿Si queremos la tabla de 8? Tenemos que hacer la alteración de los valores en diferentes lugares. <br>
    ¿Qué podemos hacer para calcular la tabla de multiplicar de otros números sin necesidad de realizar tantas alteraciones?<br>
    <br>
    <meta charset="UTF-8">
<script>
    document.write("5 por 1 es " + 5 * 1 + "<br>");
    document.write("5 por 2 es " + 5 * 2 + "<br>");
    document.write("5 por 3 es " + 5 * 3 + "<br>");
    document.write("5 por 4 es " + 5 * 4 + "<br>");
    document.write("5 por 5 es " + 5 * 5 + "<br>");
    document.write("5 por 6 es " + 5 * 6 + "<br>");
    document.write("5 por 7 es " + 5 * 7 + "<br>");
    document.write("5 por 8 es " + 5 * 8 + "<br>");
    document.write("5 por 9 es " + 5 * 9 + "<br>");
    document.write("5 por 10 es " + 5 * 10 + "<br>");
</script>   


    <br>
    <br>__________________________________________________________________________________________________________________________________________<br>
    <br>
    06 SOLUCION
    <br>
<script>
    var EDAD1 = 10;
    var EDAD2 = 20; //error corregido//
    var EDAD3 = 12;
    document.write("La media de las edades es <br>");
    document.write( (EDAD1 + EDAD2 + EDAD3) / 3);
</script>
    <br>
    <br>__________________________________________________________________________________________________________________________________________<br>
    <br>
    06 Error en comillas
    <br>
    <meta charset="UTF-8">
<script>
    var EDAD1 = 10;
    var EDAD2 = "20"; //error en comillas//
    var EDAD3 = 12;
    document.write("La media de las edades es" );
    
    document.write( (EDAD1 + EDAD2 + EDAD3) / 3);


</script>
<br>
