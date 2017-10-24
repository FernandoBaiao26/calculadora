# calculadora

using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Calcular
{
    class Program
    {
        static void Main(string[] args)
        {
            //declarando variaveis
            int n1, n2;
            double soma =0;
            int Calc = 0;

            //Entrada de dados
            Console.WriteLine("-----Calculadora------ \n");
            Console.WriteLine("Digite a Opercao");
            Console.WriteLine("(1)Soma|(2)Substracao|(3)Multiplicacao|(4)Divisao|(5)Sair \n");
            
            Calc = int.Parse(Console.ReadLine());
            

            

            if(Calc ==5)
            {

            }
            else
            {
                try
                {
                    while(Calc != 5){

                        //entrada de dados
                        
                        
                        Console.WriteLine("Digite um numero :");
                        n1 = Int32.Parse(Console.ReadLine());
                        Console.WriteLine("Digite um numero :");
                        n2 = Int32.Parse(Console.ReadLine());
                       // soma = double.Parse(Console.ReadLine());

#region Calculos
                        switch(Calc)
                        {
                            case 1:
                                soma = n1 + n2;
                                
                                break;

                            case 2:
                                soma = n1 - n2;
                                
                                break;

                            case 3:
                                soma = n1 * n2;
                                
                                break;
                            case 4:
                                soma = n1 / n2;
                                
                                break;

                            default:
                               
                                
                                break;
                           

                        }
                        #endregion
                        
                        Console.WriteLine("Resultado : " + soma);
                        
                        
                        
                        Console.ReadKey();
                        Console.WriteLine("");

                        
                       
                    }
                }
               catch(Exception ex)
                {
                   throw ex;//deixar o erro correr 
                }
            }
            Console.ReadLine();
            Console.Clear();
        }
    }
}
