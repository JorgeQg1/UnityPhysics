# UnityPhysics

En esta ocasion nos adentramos a comprobar como funciona el motor de fisicas

* ### Comprobamos el comportamiento de dos objetos sin fisicas:

  ![1o](https://user-images.githubusercontent.com/72491269/195809518-134d085c-31ff-4f58-b7c7-5b178a1b07ca.gif)

  Como podemos observar, al no ponerle fisicas a los objetos, los objetos se quedan inmoviles en su posicion inicial, sin que les afecte la gravedad.

* ### Luego le colocamos fisicas solo a la esfera:

  ![2o](https://user-images.githubusercontent.com/72491269/195812995-dc421b82-0d7f-4b3e-af76-17402b16559c.gif)

  Ahora al colocarle fisicas a la esfera comprobamos que la esfera cuenta con gravedad y todas las propiedades fisicas posibles.

* ### Ahora le colocamos fisicas a ambos objetos:

  ![3o](https://user-images.githubusercontent.com/72491269/195813946-06d27f08-7df6-4c61-a5aa-0992cc64257a.gif)

  Ahora al colocarle fisicas a ambos comprobamos que la esfera y el cubo cuentan con gravedad y todas las propiedades fisicas posibles.

* ### Lo siguiente será modificar el peso de la esfera para que pese 10 veces mas que el cubo.

  ![4o](https://user-images.githubusercontent.com/72491269/195816017-564ab10a-6968-41dd-8bfc-60947da88605.gif)

  Comprobamos que al pesar mas que antes la fuerza que ejerce sobre el cubo al caer es mucho mayor y por ello el cubo modifica su trayectoria.

* ### A continuacion la esfera tiene físicas y el cubo es de tipo IsTrigger.

  ![5o](https://user-images.githubusercontent.com/72491269/196044281-a2fb60c0-8ee9-48e1-8da4-6b0609bc8741.gif)
  
  Podemos observar como al chocar la esfera con el cubo, se detecta dentro de un metodo llamado OnTriggerEnter, el cual cambia su posicion a la inicial y le baja su velocidad a 0. Esto ocurre ya que nuestro cubo ahora mismo no actua como colisionador si no que deja pasar a traves suya cualquier objeto que pase por su posicion. Al poseer esta propiedad podemos hacer uso de tres fases que contiene dicho objeto: OnTriggerEnter, OnTriggerStay y OnTriggerExit.
  
  
