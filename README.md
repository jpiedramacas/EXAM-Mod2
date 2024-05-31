# PRUEBA PILOTO EXAMEN MÓDULO 2

Esta guía te ayudará a completar la prueba piloto del módulo 2, proporcionando instrucciones detalladas y sencillas para cada sección. Asegúrate de seguir los pasos y comandos proporcionados. Está permitido utilizar todos los recursos de internet para realizar la prueba.

## Sección 1: Configuración del Entorno de Desarrollo

### Paso 1: Configuración de una Instancia EC2 en AWS con Amazon Linux

1. **Crear una instancia EC2**:
   - Inicia sesión en la consola de AWS.
   - Ve a `Servicios > EC2` y selecciona `Lanzar instancia`.
   - Elige la AMI de `Amazon Linux 2`.
   - Selecciona el tipo de instancia, `t2.micro` (gratis en el nivel gratuito de AWS).
   - Configura el almacenamiento predeterminado y haz clic en `Revisar y lanzar`.
   - Crea un nuevo par de claves o usa uno existente y guarda el archivo `.pem`.

2. **Configurar grupos de seguridad**:
   - En la consola de AWS, navega a `EC2 > Grupos de seguridad`.
   - Selecciona el grupo de seguridad asociado a tu instancia.
   - Añade una regla de entrada para permitir el tráfico puerto 8080 y el puerto 5000.

3. **Conectar a la instancia EC2**:
   - Abre tu terminal o línea de comandos.
   - Conéctate a tu instancia con el siguiente comando, reemplazando `your-key.pem` y `ec2-xx-xx-xx-xx.compute-1.amazonaws.com` con tu archivo de clave y dirección pública de la instancia:
     ```sh
     chmod 400 your-key.pem
     ssh -i "your-key.pem" ec2-user@ec2-xx-xx-xx-xx.compute-1.amazonaws.com
     ```

### Paso 2: Instalación y Configuración de Herramientas de Desarrollo

1. **Actualizar el sistema**:
   ```sh
   sudo yum update -y
   ```

2. **Instalar Python**:
   ```sh
   sudo yum install python3 -y
   ```

3. **Instalar pip**:
   ```sh
   sudo yum install python3-pip -y
   ```

## Sección 2: Desarrollo de la Aplicación Web

### Paso 1: Creación de la Aplicación Web con Flask

1. **Instalar Flask**:
   ```sh
   pip3 install Flask
   ```

2. **Crear la estructura del proyecto**:
   ```sh
   mkdir my_flask_app
   cd my_flask_app
   ```

3. **Crear los archivos 

Perfecto, aquí tienes un ejemplo genérico de árbol de directorios para un proyecto web simple utilizando Flask:

```
proyecto_web_flask/
├── app.py
├── templates/
     └── formulario.html
```

`app.py`**
   ```python
   from flask import Flask, request, render_template_string

   app = Flask(__name__)

   @app.route('/')
   def home():
       return '¡Hola, Mundo!'

   @app.route('/form', methods=['GET', 'POST'])
   def form():
       if request.method == 'POST':
           nombre = request.form['nombre']
           return f'Hola, {nombre}!'
       return render_template_string('''
           <form method="post">
               Nombre: <input type="text" name="nombre">
               <input type="submit" value="Enviar">
           </form>
       ''')

   if __name__ == '__main__':
       app.run(host='0.0.0.0', port=8080)
   ```

Para el formulario HTML (`formulario.html`), aquí tienes un ejemplo básico:

```html
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Formulario</title>
</head>
<body>
    <h2>Formulario</h2>
    <form method="POST">
        <label for="nombre">Nombre:</label>
        <input type="text" id="nombre" name="nombre" required>
        <button type="submit">Enviar</button>
    </form>
</body>
</html>
```


5. **Ejecutar la aplicación**:
   ```sh
   sudo python3 app.py
   ```

### Paso 2: Implementación de Funcionalidades Básicas

- Añade al menos una ruta (`/` que muestra "¡Hola, Mundo!").
- Añade al menos un formulario (`/form` que acepta un nombre y muestra un saludo personalizado).

## Sección 3: Pruebas y Depuración

### Paso 1: Desarrollo de Casos de Prueba

1. **Crear el archivo `test_app.py`**:
   ```python
   import unittest
   from app import app

   class FlaskTestCase(unittest.TestCase):
       def setUp(self):
           self.app = app.test_client()
           self.app.testing = True

       def test_home(self):
           result = self.app.get('/')
           self.assertEqual(result.status_code, 200)
           self.assertIn(b'¡Hola, Mundo!', result.data)

       def test_form_get(self):
           result = self.app.get('/form')
           self.assertEqual(result.status_code, 200)
           self.assertIn(b'<form', result.data)

       def test_form_post(self):
           result = self.app.post('/form', data=dict(nombre='Estudiante'))
           self.assertEqual(result.status_code, 200)
           self.assertIn(b'Hola, Estudiante!', result.data)

   if __name__ == '__main__':
       unittest.main()
   ```

### Paso 2: Ejecución de Pruebas

1. **Ejecutar las pruebas**:
   ```sh
   python3 -m unittest test_app.py
   ```

### Conclusión

Esta guía te ha llevado a través de la configuración de una instancia EC2 en AWS, la instalación de herramientas de desarrollo, la creación de una aplicación web simple con Flask, y la implementación de pruebas automatizadas. Siguiendo estos pasos, deberías tener un entorno de desarrollo funcional y una comprensión básica del desarrollo y prueba de aplicaciones web en Python.

¡Buena suerte en tu prueba piloto!
