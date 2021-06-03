import java.lang.*;//importa, para mandar siempre a escribir en la pantalla, no es necesario escribirlo  -.-
public class Circuloss

{
    // variables de instancia 

    //¿Por qué se llaman variables de instancia ?
    //Por que cualquier objeto circulo que saquemos de la clase Circulo, va a contener una x,x,r, son variables que se
    //copian a cada uno de los objetos circulos que prodamos sacar de esta clase
    //cuando se instancia un circulo ( cuando se crea un objeto circulo), 
    //se le crean estas tres variables, que son variables de intancia,
    //pertenecen a los objetos circulo que vayamos a crear.
        
    public double x; 
    public double y;
    public double r;
    //public doible x,y,r;

    
//when the parameter and the variable of instance are the same:
//this.x=x;    :,)
//mood elegante owo'

    //{{{{{{{{{{{{{{{{{{{{{{{{{{{{{{{{{{{{{{{{{{
    //public Circuloss(double cx, double cy, double radio) //Este es un constructor, que no tiene tipo, es la unica
    //función que no tiene tipo, ni si quiera "void", no retorna nada , es una funcion que crea un objeto en memoria,
    //no me va retornar nada, va crear un objeto circulo en la memoria de la computadora y otra caracteristica es:
    //siempre es publico (no debe de llevar ni protected,ni etc, siempre publica.)

    //En java se pueden construir varios constructores, se puede definir varias formas de crear circulos
    //de forma diferente.

    public Circuloss (double radio) //otro constructor que hace lo mismo que el primero y 
    //a esto se le llama sobre carga de metodos.
    {
        x=0;
        y=0;
        r=radio;
    }

    //{
   //   x=cx;
    //  y=cy;
    //  r=radio;
    //}

    //Solo los podemos usar si usamos nuestro constructor <que.hicimos.como.progrmadores>
    //Circuloss c1=new Circuloss();
    //Circuloss c2=new Circuloss();   
    //Circuloss c3=new Circuloss();
    //Circuloss c4=new Circulos();
    //}}}}}}}}}}}}}}}}}}}}}}}}}}}}}}}}}}}}}}}}}}}}}}}}}}}}}}}}

    public Circuloss (Circuloss c)
    {
     x=c.x;
     y=c.y;
     r=c.r;   
    }
    public Circuloss ()
    //ejemplo
    //  Circulo c3= new Circulo(c1);


    //Definir las operaciones
    //En java "las operaciones" se le define como <metodos>,
    //(pero como son variables de instancia, los metodos tambien va a ser metodos de instancia xd)

    //Metodos de instancia
    //por ser una variable de instancia no se pone en los parametros, un metodo de instancia puede trabajar con cualquier
    //variable de instancia.

    double circunferencia()  
     {
     return 2*3.1416*r;
    }

    double area ()
    {
        return 3.1416*r*r;
    }
 public static void main (String args [])
    {
        Circuloss c1,c2,c3,c4; //Se define cuatro variables de tipo circulo,
                             //esto quiere decir que cada uuna de esas variables
                             //contendran 1 objeto ciirculo.
                      //cracion dee circulos       
     //todo objeto en una clase Java se crea con la palabrita new, para crear un nuevo objeto
       c1= new Circuloss(); //Asi es como es crea un objeto circulo y se alamacena en la variable c1
                        //eso significa que la varible c1 es un objeto circulo; 
                        //(la palabrita new seguido del nombre de la clase; del obejeto que quiero crear).
       c2= new Circuloss();        c3= new Circuloss();
       c4= new Circuloss();

       //otra manera de crear objetos y al mismo tiempo asignandole el tipo de variable. 
      // Circuloss c2= new Circuloss();metodo especial (construsctor) ¿Porque? -Pues porque 
      //sirve para crear objetos de tipo circulo, el constructor debe tener el mismo nombre de la clase
      //un contrustor es una funcion que permite construir un objeto.

       //Circuloss c3= new Circuloss();
       //Circuloss c4= new Circuloss();



       //Cuando yo quiera acceder a los datos de un objeto, lo voy hacer con el operador (.) 
       c1.x=2.0;// Darle valores a las variables del circulo uno.
       c1.y=1.5;
       c1.r=3.0;
       
       c2.x=8.9;//Darle valores a las variables del circulo dos.
       c2.y=9.2;
       c2.r=4.6;

       c3.x=1.5;//Darle valores a las variebles del circulo tres.
       c3.y=9.5;
       c3.r=5.3;

       c4.x=9.8;//Darle valores a las variables del circulo cuatro.
       c4.y=6.2;
       c4.r=9.4;
       //otra forma, es decir; 
       //double a=c1.area();
       //double c=c1.circunferencia();   

       //System.out.println("Coordenadas x,y del circulo c1= ("+c1.x+","+c1.y+")   y radio"+c1.r+"\n");//concatenar
       //System.out.println("Area del circulo C1="+a);
       //System.out.println("Circuferencia del circulo C1="+c);

       System.out.println("Coordenadas x,y del circulo c1= ("+c1.x+","+c1.y+")   y radio"+c1.r+"\n");//concatenar
       System.out.println("Area del circulo C1="+c1.area());
       System.out.println("Circuferencia del circulo C1="+c1.circunferencia());
       System.out.println ("Coordenadas x,y del circulo c2= ("+c2.x+","+c2.y+") y el radio es:"+c2.r+"\n");
       System.out.println("Area del circulo C2=" +c2.area());
       System.out.println ("Circunferencia del circulo C2="+c2.circunferencia());
       System.out.println("Coordenadas x,y del circulo c3= ("+c3.x+","+c3.y+")  y el radio es:"+c3.r+"\n");
       System.out.println("Area del circulo C3=" +c3.area());
       System.out.println("Circunferencia del circulo C3="+c3.circunferencia());
       System.out.println("Coordenadas x.y del circulo c4= ("+c4.x+","+c4.y+")  y el radio es: "+c4.r+"\n");
       System.out.println("Area del circulo c4="+c4.area());
       System.out.println("Circunferencia del circulo C4="+c4.circunferencia());

       //println (lo que hace el println es mandar excribir la cadena y como tiene el "ln" automaticamente
       //tiene retorno de carro
       //tambien se puede usar solamente "print"

       //para los que les cuesta dejar c  :v
       System.out.printf("\nCoordenada x,y del circulo C1= (%f, %f) y radio= %f\n", c1.x,c1.y,c1.r);


       //incompleto





    }
}
