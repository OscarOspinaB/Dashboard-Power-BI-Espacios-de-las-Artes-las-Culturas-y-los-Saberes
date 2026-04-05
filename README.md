# Dashboard-Power-BI-Espacios-de-las-Artes-las-Culturas-y-los-Saberes

Mínimo producto viable, se espera actualizar el informe con mejoras proximamente.

# 📊 [Click_Dashboard_interactivo](https://app.powerbi.com/view?r=eyJrIjoiY2I2NTRiMzUtMzI1Ny00MDFlLWE0ZDItZWQ1NzI3MzY1Y2IxIiwidCI6Ijk5ZTFlNzIxLTcxODQtNDk4ZS04YWZmLWIyYWQ0ZTUzYzFjMiIsImMiOjR9)

## Fuente de los datos
Los datos utilizados fueron obtenidos de [datos.gov](https://www.datos.gov.co/Cultura/Espacios-de-las-Artes-las-Culturas-y-los-Saberes/te39-v28f/about_data)

Sino pueden acceder al link, simplemente copiar y pegar el siguiente enlace:
https://www.datos.gov.co/Cultura/Espacios-de-las-Artes-las-Culturas-y-los-Saberes/te39-v28f/about_data

<img width="1867" height="692" alt="image" src="https://github.com/user-attachments/assets/88ce2457-fb98-4840-addb-ef0b5086f2e0" />


Para la conexión con los datos utilicé la siguiente configuración de la API para exportar los datos formato Json

<img width="1388" height="845" alt="image" src="https://github.com/user-attachments/assets/05ed6a3a-ee20-4480-977c-0d7dfdb5aa0b" />

Cómo se puede apreciar en la imagen anterior, solo importé 1000 datos por defecto de la API por practicidad y límitaciones del equipo local donde se realizó el Dashboard, no obstante, si se requiere aumentar el límite de datos para que así el informe contenga el total de los datos reales del dataset. Para ello, agregamos a lo siguiente al enlace de la API que copiemos al exportar los datos de DatosGov :

## ?$limit=30000
Nota: en el código anterior se aprecia que el límite de filas o registros es de treinta mil

Si se desea conocer cómo aumentar el límite de filas o registros que se pueden exportar al Power BI, ir al final del texto.
A modo de ejemplo se muestra la guía para aumentar el límite de filas:

* Suponga que exportÓ el siguiente enlace de la API:
<img width="786" height="778" alt="image" src="https://github.com/user-attachments/assets/27c51238-b23d-4466-a152-4ab6a8de27d0" />

* Por defecto, tenemos 1000 filas para exportar, con lo cual establecemos manualmente el límite de filas a 30000 copiando y pegando #?$limit=30000

  https://www.datos.gov.co/resource/te39-v28f.json?$limit=30000

Lo anterior sirve para incrementar el límite de registros que exportas al Power BI.
---
# 01 Vistazo General Dashboard
Cabe señalar que se puede desplazar por el mapa a gusto personal, así como aplicar zoom en el mismo
<img width="1198" height="683" alt="image" src="https://github.com/user-attachments/assets/9b72f365-4371-434a-8572-1be6a0736e26" />


# 02 Tooltip

<img width="739" height="710" alt="image" src="https://github.com/user-attachments/assets/4015d95f-6e06-4f44-9aa2-1762bef81043" />


# 03 Ejm filtro por departamento 'Antioquia'

<img width="1205" height="681" alt="image" src="https://github.com/user-attachments/assets/b737cf4d-db68-4769-b488-2abe3331a6ca" />


# 04 Ejm filtro por departamento 'Antioquia' y ciudad 'Medellín'
<img width="1206" height="683" alt="image" src="https://github.com/user-attachments/assets/5a62f813-60e8-4b72-93c0-3d7d013e6711" />


---
# Aumentar el límite de filas a exportar de la API de DatosGov

A modo de ejemplo se muestra la guía para aumentar el límite de filas:

* Suponga que exportÓ el siguiente enlace de la API:
<img width="786" height="778" alt="image" src="https://github.com/user-attachments/assets/27c51238-b23d-4466-a152-4ab6a8de27d0" />

* Por defecto, tenemos 1000 filas para exportar, y tenemos el siguiente enlace de ejemplo:
  https://www.datos.gov.co/resource/te39-v28f.json

* Establecemos manualmente el límite de filas a 30000 copiando y pegando **?$limit=30000**

  https://www.datos.gov.co/resource/te39-v28f.json?$limit=30000

  Si ya teniamos un dashboard elaborado como es mi caso, es suficiente con abrir PowerQuery, buscar el paso de Origen y pegar ya sea el nuevo enlace o simplemente el añadido, que particularmente consideró más eficiente de hacer:

  **?$limit=30000**
* Abrir Power Query, editamos el paso de **Origen**
  
  <img width="1453" height="471" alt="image" src="https://github.com/user-attachments/assets/7b0cab96-a2ba-49f5-92d4-16a98ba51480" />

* Añadimos lo siguiente al final del enlace JSON: **?$limit=30000**, click en aceptar

  <img width="1068" height="498" alt="image" src="https://github.com/user-attachments/assets/6ba5fce3-1590-44b2-9def-5c4e19754221" />


Dado que mi equipo presenta limitaciones para aumentar a esa cantidad de datos, se mantendrá el Dashboard tal cuál está

