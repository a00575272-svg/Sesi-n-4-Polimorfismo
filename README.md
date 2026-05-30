1#¿Cuál es la diferencia entre polimorfismo en tiempo de compilación y en tiempo de ejecución?
Tiempo de compilación: La decisión sobre qué función utilizar se toma antes de ejecutar el programa. Se logra mediante la sobrecarga de funciones y operadores.
Tiempo de ejecución: La decisión se toma mientras el programa se está ejecutando. Se utiliza con funciones virtuales y herencia, permitiendo que se invoque la versión correspondiente al tipo real del objeto.

2#¿Para qué sirve la palabra virtual?
La palabra clave virtual indica que un método puede ser redefinido en una clase derivada y que la llamada al método se resolverá en tiempo de ejecución según el tipo real del objeto.

3#¿Qué ventaja tiene usar override?
override permite indicar explícitamente que un método está sobrescribiendo un método virtual de la clase base. Esto ayuda a detectar errores de programación, ya que el compilador verifica que realmente exista un método compatible para sobrescribir.

4#¿Por qué una clase con un método = 0 se considera abstracta?
Porque un método declarado con = 0 es una función virtual pura, lo que obliga a las clases derivadas a implementarla. Una clase que contiene al menos una función virtual pura no puede instanciarse directamente y se considera abstracta.

5#¿Por qué se recomienda usar destructor virtual en clases base?
Porque garantiza que, al eliminar un objeto derivado mediante un puntero de la clase base, se ejecuten correctamente tanto el destructor de la clase derivada como el de la base. Esto evita fugas de memoria y problemas de liberación de recursos.

6#¿Qué significa que un puntero de clase base apunte a un objeto derivado?
Significa que una variable puntero del tipo de la clase base almacena la dirección de un objeto de una clase que hereda de ella. Esto permite aplicar polimorfismo, ya que mediante el puntero base se pueden llamar métodos virtuales que ejecutarán la versión correspondiente de la clase derivada.

Evidencia de codigo <img width="426" height="445" alt="image" src="https://github.com/user-attachments/assets/fc5f8c4d-3cf2-4e98-86f1-95c5fe411552" />
