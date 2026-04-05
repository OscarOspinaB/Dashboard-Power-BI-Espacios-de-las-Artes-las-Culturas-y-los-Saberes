# Dashboard-Power-BI-Espacios-de-las-Artes-las-Culturas-y-los-Saberes

Mínimo producto viable, se espera actualizar el informe proximamente.

# 📊 [Click_Dashboard_interactivo](https://app.powerbi.com/view?r=eyJrIjoiY2I2NTRiMzUtMzI1Ny00MDFlLWE0ZDItZWQ1NzI3MzY1Y2IxIiwidCI6Ijk5ZTFlNzIxLTcxODQtNDk4ZS04YWZmLWIyYWQ0ZTUzYzFjMiIsImMiOjR9)

## Fuente de los datos
Los datos utilizados fueron obtenidos de [datos.gov](https://www.datos.gov.co/Cultura/Espacios-de-las-Artes-las-Culturas-y-los-Saberes/te39-v28f/about_data)

Sino pueden acceder al link, simplemente copiar y pegar el siguiente enlace:
https://www.datos.gov.co/Cultura/Espacios-de-las-Artes-las-Culturas-y-los-Saberes/te39-v28f/about_data

<img width="1867" height="692" alt="image" src="https://github.com/user-attachments/assets/88ce2457-fb98-4840-addb-ef0b5086f2e0" />


Para la conexión con los datos utilicé la siguiente configuración de la API para exportar los datos formato Json

<img width="1388" height="845" alt="image" src="https://github.com/user-attachments/assets/05ed6a3a-ee20-4480-977c-0d7dfdb5aa0b" />

Cómo se puede apreciar en la imagen anterior, solo importé 1000 datos por defecto de la API por practicidad, no obstante, si se requiere aumentar el límite de datos para que así el informe contenga el total de los datos reales del dataset. Para ello, agregamos a lo siguiente al enlace de la API que copiemos al exportar los datos de DatosGov :

## ?$limit=30000
Nota: en el código anterior se aprecia que el límite de filas o registros es de treinta mil

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




