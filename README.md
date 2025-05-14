# pruebaclase
prueba de crear un repo en clase

cambios para forzar un ejemplo

## Ejemplos de las diferentes opciones que brinda el formato Markdown

# Texto en H1
## Texto en H2
### Texto en H3
#### Texto en H4
##### Texto en H5
###### Texto en H6

---
Línea separadora
---


Se puede definir texto en *cursiva*, **negrita** o ***ambas***

Se puede definir `código o palabras clave en una línea`

o definir bloques de código entero

```java
// Ejemplo de código en Java

@DeleteMapping("/{id}")
    public ResponseEntity<?> remove(@PathVariable Long id){
        Optional<Grupo> optGrupo = service.findById(id);
        if (optGrupo.isPresent()){
            service.delete(id);
            return ResponseEntity.noContent().build();
        }
        return ResponseEntity.notFound().build();
    } 
```

```python
# Ejemplo de código en Python

def process_directory(input_dir, extension='jpg'):
    output_dir = os.path.join(input_dir, 'transparent_bg_rembg')
    os.makedirs(output_dir, exist_ok=True)

    for filename in os.listdir(input_dir):
        if filename.lower().endswith(f'.{extension.lower()}'):
            rutaOrigen = os.path.join(input_dir, filename)
            output_filename = f"no_bg_{os.path.splitext(filename)[0]}.png"  # Siempre PNG
            rutaDestino = os.path.join(output_dir, output_filename)
            procesarImagen(rutaOrigen, rutaDestino)
```

> [!Note] 
> ### Se puede definir una sección de notas
> - nota 1
> - nota 2
> - nota 3
>

> [!Note] 
> ### Las notas pueden incluir bloques de código
> ```python
> rutaDestino = os.path.join(output_dir, output_filename)
> procesarImagen(rutaOrigen, rutaDestino)
> ```

## Tipos de notas que podemos usar

> [!NOTE]
> Información que pueda merecer la pena tener en cuenta

> [!TIP]
> Consejos, buenas prácticas o cualquier información que pueda ser de ayuda

> [!IMPORTANT]
> Información que queramos remarcar como muy necesaria o crucial

> [!WARNING]
> Avisos a tener en cuenta aunque no sean errores, riesgos potenciales

> [!CAUTION]
> Catástrofe inminente, se va a liar, peligro asegurado, error garantizado... ¿sigo?


