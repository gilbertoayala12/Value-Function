package ecuacion;

import java.util.*;
import javax.script.ScriptEngineManager;
import javax.script.ScriptEngine;
import javax.script.ScriptException;

/**
 *
 * @author Gilberto
 */
public class Ecuacion {

    /**
     * @param args the command line arguments
     */
    public static int letra = 0;
    public static int num = 0;
    public static int oper = 0;
    public static int[] numArray;
    public static String[] stringArray;
    public static String[] secondArray;

    public static void main(String[] args) throws ScriptException {
        ScriptEngineManager eng = new ScriptEngineManager();
        ScriptEngine engine = eng.getEngineByName("JavaScript");
        Scanner n = new Scanner(System.in);
        System.out.print("Ingresa una expresion matematica:" + " ");
        String exp = n.nextLine();
        System.out.println(exp);
        stringArray = exp.split("=");
        String split_oper = stringArray[1];
        String seg_split;
        tipoDe(exp);
        letra(letra);
        operador(oper);
        numero(num);
        System.out.println("Dame el valor que le quieras dar a la variable");
        String valorString = n.nextLine();
        char valor = valorString.charAt(0);

        if (exp.contains("/")) {

            for (int i = 0; i < split_oper.length(); i++) {
                if (Character.isLetter(split_oper.charAt(i))) {
                    char[] array = split_oper.toCharArray();
                    array[i] = valor;
                    split_oper = String.valueOf(array);
                    System.out.print("La division es " + split_oper + " y el resultado es ");
                    break;
                }
            }

            String inDiv = split_oper;
            System.out.println(engine.eval(inDiv));
        } else if (exp.contains("+")) {
            for (int i = 0; i < split_oper.length(); i++) {
                if (Character.isLetter(split_oper.charAt(i))) {
                    char[] array = split_oper.toCharArray();
                    array[i] = valor;
                    split_oper = String.valueOf(array);
                    System.out.print("La suma es " + split_oper + " y el resultado es ");
                    break;
                }
            }

            String inDiv = split_oper;
            System.out.println(engine.eval(inDiv));

        } else if (exp.contains("-")) {
            for (int i = 0; i < split_oper.length(); i++) {
                if (Character.isLetter(split_oper.charAt(i))) {
                    char[] array = split_oper.toCharArray();
                    array[i] = valor;
                    split_oper = String.valueOf(array);
                    System.out.print("La resta es " + split_oper + " y el resultado es ");
                    break;
                }
            }

            String inDiv = split_oper;
            System.out.println(engine.eval(inDiv));

        } else if (exp.contains("*")) {
            for (int i = 0; i < split_oper.length(); i++) {
                if (Character.isLetter(split_oper.charAt(i))) {
                    char[] array = split_oper.toCharArray();
                    array[i] = valor;
                    split_oper = String.valueOf(array);
                    System.out.print("La multiplicacion es " + split_oper + " y el resultado es ");
                    break;
                }
            }

            String inDiv = split_oper;
            System.out.println(engine.eval(inDiv));

        }

    }

    public static void letra(int x) {
        if (x > 1) {
            System.out.println("Hay " + x + " constantes");
        } else {
            System.out.println("Hay " + x + " constante");
        }
    }

    public static void tipoDe(String x) {
        for (int i = 0; i < x.length(); i++) {
            if (Character.isLetter(x.charAt(i))) {

                letra++;
            } else if (Character.isDigit(x.charAt(i))) {

                num++;
            } else {

                oper++;
            }
        }
    }

    public static void operador(int x) {
        if (x > 1) {
            System.out.println("Hay " + x + " operadores contando parentesis");
        } else {
            System.out.println("Hay " + x + " operador");
        }
    }

    public static void numero(int x) {
        if (x > 1) {
            System.out.println("Hay " + x + " numeros");
        } else {
            System.out.println("Hay " + x + " numeros");
        }
    }
}
