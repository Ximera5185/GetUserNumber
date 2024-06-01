# GetUserNumber
 private int GetUserNumber(string message)
 {
     int number = 0;

     string input = "";

     bool isNumber = false;

     while (isNumber == false)
     {
         Console.WriteLine(message);

         input = Console.ReadLine();

         isNumber = int.TryParse(input, out number);

         if (isNumber == false)
             Console.WriteLine("Вы ввели не целое число.");
         else
             isNumber = true;

         Console.Clear();
     }

     return number;
 }
