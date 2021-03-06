# Estruturas de dados Heterogêneas(struct)

+ As estruturas de dados (Homogêneas e Heterogêneas) possibilitam a construção de estruturas mais complexas que os tipos de dados primitivos (int, char,..).
+ Diferentemente dos tipos homogêneos, essas estrturas permitem a manipulação de um conjunto de informações de tipos de dados primitivos diferentes, mas que possuem um relacionamento lógico entre si;
+ Exemplo de um registro de Funcionário
![programa](/markdowns/registro.png)
+ O Registro acima possui um conjunto informações relacionadas a um funcionário, logo poderiam ser vistas agrupadas num único nome (como as Matrizes).
+ A linguagem C possui uma estrutura denominada <b>struct</b> que permite agrupar um conjunto de informações de tipos diferentes cob um mesmo nome.
 ```
 Declaração:
     struct {
       tipo_de_dado1 <Nome das Varáveis1>;
       tipo_de_dado2 <Nome das Variáveis2>;
       ....
       tipo_de_dadoN <Nome das VariáveisN>;
     } nome_Variavel_struct;
     
     Exemplo:
      struct{
       int    matricula;
       string nome[30];
       string dataNasc[9];
       string cargo[20];
       float  salario
     }func;
 ```
 + A variável <b>func</b> é do tipo registro (struct) e, para individualizar cada dado (nesse caso é denominado de campo), basta colocar o nome da variável seguido de um ponto seguido com o nome do campo.
    ex: <b>func.matricula</b>
+ O exemplo a seguir cria a estrutura funcionário, lê as informações de cada um dos campos e exibe o que foi lido.

@[IDE]({"stubs": ["./www/estrutura"],"command": "sh /project/target/www/estrutura.sh" })

