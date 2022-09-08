<h1 align="center">Primeiro Programa em JAVA</h1>

<p>Crie um novo arquivo em seu editor de texto ou IDE (<a href="https://www.jetbrains.com/pt-br/idea/download/#section=windows">recomendo o INTELLIJ</a>) chamado <strong>OlaMundo.java</strong>. Em seguida, escreva este bloco de código no arquivo e salve (tente digitar por si mesmo, evite copiar e colar):</p>

<blockquote>public class OlaMundo {<br>
public  static  void  main(String[]  args)  { <br>
System.out.println("Ola, Mundo!");<br>
  }<br>
}<br>
</blockquote>
<br>
<p><i><strong>Nota:</strong> Para que o Java reconheça isso como uma <strong>classe pública</strong> (e não lançar um erro de tempo de compilação), o nome do arquivo deve ser o mesmo que o nome da classe (OlaMundo neste exemplo) com uma extensão .java.</i></p>
<br>
<p>Se você está criando o código em um editor de texto e já o salvou com a extensão .java, agora vamos executá-lo. Copie o endereço de onde o arquivo está salvo, caso salvou na área de trabalho, um exemplo de como ficaria: "C:\Users\xxx\Área de Trabalho\OlaMundo.java". Agora abra o Prompt de Comando, digite java + o link para o arquivo e pressione a tecla enter. O resultado no seu Prompt de Comando será a frase "Ola, Mundo!".</p>
<p>Caso você tenha escrito no <strong>INTELLIJ</strong> (o qual passaremos a usar a partir de agora), basta clicar na setinha verde ao lado do seu código e a frase "Ola, Mundo!" será impressa na parte inferior do programa. Caso aconteça algum erro, o programa avisará.</p>

<p>Parabéns, você compilou seu primeiro programa em JAVA! Agora vamos entender melhor o que você escreveu para que chegasse nesse resultado.</p>

<h1 align="center">Conceituando o Código Escrito</h1>

<p>O programa "Ola, Mundo" contém um único arquivo, que consiste em uma <strong>definição de classe</strong> OlaMundo, um método <strong>main</strong> e uma instrução dentro do método main.</p>
<br>
<blockquote>public class OlaMundo {</blockquote>
<p>A palavra-chave <strong>class</strong> inicia a definição de classe para uma classe chamada OlaMundo. Cada aplicação Java contém pelo menos uma definição de classe.</p>
<br>
<blockquote>public  static  void  main(String[]  args)  {</blockquote>
<p>Este é um método de ponto de entrada (definido por seu nome e assinatura de public static void main(String[])) a partir do qual a JVM (Java Virtual Machine) pode executar seu programa. Todo programa Java deve ter um. Isso é:</p>
<li><strong>public:</strong> significando que o método pode ser chamado de qualquer lugar, de fora do programa também;
<li><strong>static:</strong> significa que ele existe e pode ser executado sozinho (no nível de classe sem criar um objeto);
<li><strong>void:</strong> significa que não retorna nenhum valor. <i><strong>Nota:</strong> Isso é diferente de C e C++ onde um código de retorno como int é esperado (o modo de Java é System.exit()).</i></li>

<p>O método <strong>main</strong> aceita></p>
<li>Uma matriz (normalmente chamada de <i>args</i>) de <i>Strings</i> passadas como argumentos para a função principal (por exemplo, de argumentos de linha de comando).</li>

<p>Quase tudo isso é necessário para um método de ponto de entrada Java. As vezes as coisas podem parecer assustadoras, muitos códigos, muitas frases, mas não precisa se preocupar, tudo fica mais fácil com o tempo. Às vezes temos medo do desconhecido, mas o Java está aqui para ser um amigo e com dedicação você vai tirar tudo de letra fácil, fácil.</p>
<p>Partes não obrigatórias:</p>
<li>O nome args é um nome de variável, portanto, pode ser chamado como você quiser, embora seja normalmente chamado de args;
<li>Se seu tipo de parâmetro é um <i>array</i> (String[] args) ou <i>Varargs</i> (String... args) não importa porque arrays podem ser passados para varargs (não se preocupe com isso agora, veremos sobre <strong>varargs</strong> futuramente, ele merece um tópico só para ele).</li>

<p><i><strong>Nota:</strong> Um único aplicativo pode ter várias classes contendo um método de ponto de entrada (principal). O ponto de entrada do aplicativo é determinado pelo nome da classe passado como argumento para o comando java.</i></p>

<p>Dentro do método <strong>main</strong>, vemos a seguinte declaração:</p>
<blockquote>System.out.println("Ola, Mundo!");</blockquote>
<p>Vamos dividir esta declaração elemento por elemento:</p>
<ul><strong>System:</strong> isso denota que a expressão subsequente chamará a classe System, do pacote <i>java.lang</i>.</ul>
<ul><strong>.:</strong> este é um "operador de ponto". Os operadores de ponto fornecem acesso a uma classe <i>member1</i>; ou seja, seus campos
. (variáveis) e seus métodos. Neste caso, este operador de ponto permite que você faça referência ao campo estático <i>out</i> dentro da classe <i>System</i>.</ul>
<ul><strong>out:</strong> este é o nome do campo estático do tipo <i>PrintStream</i> dentro da classe <i>System</i> que contém a funcionalidade de saída padrão.</ul>
<ul><strong>.:</strong> este é outro operador de ponto. Este operador de ponto fornece acesso ao método <i>println</i> dentro da variável <i>out</i>.</ul>
<ul><strong>println:</strong>este é o nome de um método dentro da classe <i>PrintStream</i>. Este método em particular imprime o conteúdo dos parâmetros no console e insere uma nova linha depois. Se você digitar apenas <strong>print</strong>, ele não pula uma linha.</ul>
<ul><strong>(:</strong> esse parêntese indica que um método está sendo acessado (e não um campo) e inicia os parâmetros sendo passados para o método <i>println</i>.</ul>
<ul><strong>"Ola, Mundo!":</strong> este é o literal <i>String</i> que é passado como parâmetro, no método <i>println</i>. As aspas duplas em cada extremidade delimitam o texto como uma <i>String</i>.</ul>
<ul><strong>):</strong> este parêntese significa o fechamento dos parâmetros que estão sendo passados para o método <i>println</i>.</ul>
<ul><strong>;:</strong> este ponto e vírgula marca o fim da instrução.</ul>

<p><i><strong>Nota:</strong> Cada instrução em Java deve terminar com um ponto e vírgula (;).</i></p>

<p>O corpo do método e o corpo da classe são então fechados.</p>
<blockquote>
}	// fim do escopo da função principal (main)<br>
}	// fim do escopo da classe "Ola, Mundo"
</blockquote>

<p>Você pode usar // para fazer comentários em sua aplicação Java.</p>
