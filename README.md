# PlusCycle

πλνκΈ° μ¬μ΄ν΄ λ¬Έμ  <br>
πhttps://www.acmicpc.net/problem/1110 <br>
<pre><code>using System;

namespace baekjoon
{
    class PlusCycle
    {
        static void Pcycle()
        {
            String input = Console.ReadLine();
           
                if (int.Parse(input) < 10)
                {
                    input = input + 0;
                }
            
                int orinInput = int.Parse(input);
                int cnt = 0;
                int addNum;

                while(true)
                {
                    cnt++;
                    int Fst = int.Parse(input) / 10;
                    int Sec = int.Parse(input) % 10;
                    addNum = Fst + Sec;
                    input = Sec.ToString() + (addNum % 10).ToString();
                    if (int.Parse(input) == orinInput) break;
                }
                Console.WriteLine(cnt);
        }

        static void Main(string[] args)
        {
            Pcycle();
        }
    }
}</code></pre>
πμ€λ μ½λ©νλ©° μμ¬μ λ λΆλΆμ ifλ¬Έμ μ€κ΄νΈ μμΉλ₯Ό μ λλ‘ νμΈνμ§ λͺ»ν΄ 20λΆ μ¦μμ μκ°μ νλΉνλ€λ μ  μλλ€...π λ€μμλ κ°μ μ€μλ₯Ό λ°λ³΅νμ§ μκΈ°!!! λ‘ λ€μ§νμ΅λλ€...!!!!<br>
