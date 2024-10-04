### Descripción del Caso

Se ha solicitado crear un software para gestionar la creación de personajes en un videojuego. Este sistema debe permitir la distribución de puntos entre los atributos del personaje y la gestión de habilidades. Las funcionalidades necesarias son:

1. **Asignar puntos**: Permitir al usuario asignar un número limitado de puntos entre los tres atributos (agilidad, fuerza e inteligencia).
2. **Editar puntos**: Modificar la distribución de puntos asignados previamente en los atributos.
3. **Quitar puntos**: Permitir al usuario retirar puntos de un atributo y reasignarlos si es necesario.
4. **Mostrar puntos restantes**: Mostrar al usuario cuántos puntos le quedan disponibles para asignar.
5. **Mostrar habilidades**: Permitir al usuario ver el conjunto de habilidades que el personaje ha aprendido.
6. **Agregar habilidad**: Incorporar una nueva habilidad al conjunto de habilidades del personaje.
7. **Remover habilidad**: Eliminar una habilidad específica del conjunto de habilidades del personaje.
8. **Mostrar atributos**: Presentar los valores actuales de los tres atributos del personaje.

### Requisitos Adicionales

- **Gestión de habilidades**: Implementar validaciones que aseguren que no se puedan agregar habilidades duplicadas ni eliminar habilidades que no existan.
- **Pruebas unitarias (PU)**: Desarrollar pruebas para validar el correcto funcionamiento de las funcionalidades, asegurando que tanto la distribución de puntos como la gestión de habilidades sean precisas y robustas.

### Clases

```java
import java.util.ArrayList;
import java.util.List;

public class Personaje {
    private String nombre;
    private int agilidad;
    private int fuerza;
    private int inteligencia;
    private int puntosRestantes;
    private List<String> habilidades;

    // Constructor
    public Personaje(String nombre, int puntosIniciales) {
        this.nombre = nombre;
        this.agilidad = 0;
        this.fuerza = 0;
        this.inteligencia = 0;
        this.puntosRestantes = puntosIniciales;
        this.habilidades = new ArrayList<>();
    }

    public String getNombre() {
        return nombre;
    }

    public void setNombre(String nombre) {
        this.nombre = nombre;
    }

    public int getAgilidad() {
        return agilidad;
    }

    public void setAgilidad(int agilidad) {
        this.agilidad = agilidad;
    }

    public int getFuerza() {
        return fuerza;
    }

    public void setFuerza(int fuerza) {
        this.fuerza = fuerza;
    }

    public int getInteligencia() {
        return inteligencia;
    }

    public void setInteligencia(int inteligencia) {
        this.inteligencia = inteligencia;
    }

    public int getPuntosRestantes() {
        return puntosRestantes;
    }

    public void setPuntosRestantes(int puntosRestantes) {
        this.puntosRestantes = puntosRestantes;
    }

    public List<String> getHabilidades() {
        return habilidades;
    }

    public void setHabilidades(List<String> habilidades) {
        this.habilidades = habilidades;
    }

    public String mostrarAtributos() {
    }

    public int mostrarPuntosRestantes() {
    }

    public List<String> mostrarHabilidades() {
    }
}


```
