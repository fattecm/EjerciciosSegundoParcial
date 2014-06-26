EjerciciosSegundoParcial
========================

24 Ejercicios de Web

/*EJERCICIO 3*/
function EjerTres($num1, $num2) {
    // se hace algo
    $var=0;
    $ban=0;
    if($num1==0 || $num2==0 ||$num1<=-1 || $num2<=-1 ||$num1>255 || $num2>255){
        echo '-1';   
    }else{
        $div=1;
        while($ban==0){ 
            $var= $num1*(1/$div);
            if($div==$num2)
                $ban=1;
            $div++;
        }
        echo $var;
    }
    
}

EjerTres(-5, 10)."<br>";

/*EJERCICIO 6

 * 
 *  */

function EjerSeis($cadena){
    $palabra="";
    //Con el parámetro 1 guardamos las palabras en un array. Las palabras son accesibles mediante el índice del array, 
    $array_cadena = str_word_count($cadena, 1);
    //str_word_count($cadena, 0) nos devuelve el numero de palabras
    $npalabras=str_word_count($cadena, 0);
    for($i=0;$i<=str_word_count($cadena, 0);$i++)
    {
        $palabra=$array_cadena[$npalabras];
        echo $palabra." ";
        $npalabras--;
    }
}    

EjerSeis("esta es una prueba")."<br>";
