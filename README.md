# Yasmim

string nomeItemUm="Hamburguer Artesanal", nomeItemDois="Refrigerante", nomeItemTres="Batata Frita";
double vlItemUm= 29.90, vlItemDois= 134.90, vlItemTres= 189.00, percentualImposto= 0.088, vlTotalCliente, impostoCliente, totalComImposto;
int qtdItemUm, qtdItemDois, qtdItemTres;

Console.WriteLine("Bem-Vindo a Lanchonete Delicia \n");
Console.WriteLine("+======================================================+");
Console.WriteLine("|                   Lanchonete Delicia                 |");
Console.WriteLine("+======================================================+");
Console.WriteLine("|                       Cardapio                       |");
Console.WriteLine("+======================================================+");
Console.WriteLine("|       Item                              Valor        |");
Console.WriteLine("+======================================================+");
Console.WriteLine($"|1.{nomeItemUm}                     {vlItemUm}       |");
Console.WriteLine($"|2.{nomeItemDois}                             {vlItemDois}      |");
Console.WriteLine($"|3.{nomeItemTres}                             {vlItemTres}        |");
Console.WriteLine("+======================================================+");

Console.WriteLine("Por favor digite a quantidade que deseja do primeiro item:");
qtdItemUm = Convert.ToInt32(Console.ReadLine()!);
Console.WriteLine("Por favor digite a quantidade que deseja do primeiro item:");
qtdItemDois = Convert.ToInt32(Console.ReadLine()!);
Console.WriteLine("Por favor digite a quantidade que deseja do primeiro item:");
qtdItemTres = Convert.ToInt32(Console.ReadLine()!);

vlItemUm = qtdItemUm * vlItemUm;

vlItemDois = qtdItemDois * vlItemDois;

vlItemTres = qtdItemTres * vlItemTres;

vlTotalCliente = vlItemDois + vlItemTres + vlItemUm;

impostoCliente = percentualImposto * vlTotalCliente;

totalComImposto = vlTotalCliente + impostoCliente;

Console.WriteLine("\n+======================================================+");
Console.WriteLine("|                    Recibo de Compra                  |");
Console.WriteLine("+======================================================+");
Console.WriteLine("|       Item                              Valor        |");
Console.WriteLine("+======================================================+");
Console.WriteLine($"|{qtdItemUm} x {nomeItemUm}               {vlItemUm:F2}          |");
Console.WriteLine($"|{qtdItemDois} x {nomeItemDois}                        {vlItemDois:F2}          |");
Console.WriteLine($"|{qtdItemTres} x {nomeItemTres}                        {vlItemTres:F2}         |");
Console.WriteLine("+======================================================+");
Console.WriteLine($"| Valor Total sem imposto: {vlTotalCliente:F2}                      |");
Console.WriteLine($"| Imposto (8,8%) {impostoCliente:F2}                                 |");
Console.WriteLine($"| Valot Total Com Imposto: {totalComImposto:F2}                      |");
Console.WriteLine("+======================================================+");
Console.WriteLine($"| Valor Total a Pagar:{totalComImposto:F2}                           |");
Console.WriteLine("+======================================================+");
