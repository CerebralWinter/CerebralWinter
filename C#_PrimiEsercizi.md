MODULO OOP -LINGUAGGIO C# -COMPITO2

Realizzare un’applicazione di tipo Console e di nome Ese2 che abbia le seguenti caratteristiche: 

Deve poter essere eseguita da finestra di comando (Console) nei modi:


Ese2 <numero: un numero>

Ese2<testo: nome persona> <numero: temperatura corporea>

Nel caso con un solo parametro l’applicazione dovrà stampare a schermo in colonna i numeri interi da 0 a numero.

Nel caso con due parametri l’applicazione dovrà stampare a schermo la seguente frase:

Ciao testo, la tua temperatura è numero e frase finale!

dove frase finale varrà:

●Per temperatura < 35: e sei in ipotermia

●Per temperature maggiori o uguali a 35 e minori di 38: e stai bene

●Per temperature maggiori o uguali a 38: e hai la febbre

```c#
static void Main(string[] args)
        {

            if (args.Length == 1 && int.TryParse(args[0], out int n))
            {
                for (int i = 0; i <= n; i++)
                {
                    Console.WriteLine(i);
                }

            }
            else if (args.Length == 2 && !int.TryParse(args[0], out n) && int.TryParse(args[1], out n))
            {
                string fraseFinale = "";
                if (n < 38 && n >= 35)
                    fraseFinale = "e stai bene";
                else if (n < 35)
                    fraseFinale = "e sei in ipotermia";
                else if (n >= 38)
                    fraseFinale = "e hai la febbre";
                Console.WriteLine("Ciao {0}, la tua temperatura è {1} {2}", args[0], args[1], fraseFinale);
            }
            else
                Console.WriteLine("Esegui il programma da cmd. Dopo aver digitato il nome dell'eseguibile dalla working directory in cui si trova, digitare un numero e premere invio, o una parola ed un numero. Negli altri casi si visualizzerà questo messaggio.");

            Console.ReadKey();
        }
```