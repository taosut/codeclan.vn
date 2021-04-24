---
title: "Cómo generar un setup B2B super accionable"
description: "Un análisis sobre un sistema de generación de leads y cotizaciones que desarrollamos junto a un cliente del rubro de limpieza de ductos y purificación de aire."
date: 2020-05-02T20:22:20-03:00
draft: false
---

Este contenido surge de un caso real para un experimento para un cliente de WhoKnows.

**El desafío era:** obtener una base de jefes de mantenimiento en todo México para contactarlos por Linkedin y a su vez tratar de conseguir sus mails para hacerles un approach personalizado y conseguir reuniones para cotizar limpiezas de ductos de aires acondicionados.

Usamos las siguientes herramientas:

- Texau / Phantombuster
- One2Lead 
- Sales Navigator
- Gmass 
- FindThatLead

Lo primero que hicimos con este caso fue utilizar Sales Navigator para obtener un mapeo general de empresas dentro de México.

En este caso buscábamos contactar a Farmacias, Supermercados y pequeñas empresas similares con atención al público que tengan sucursales.

Generamos listas de búsquedas de Sales Navigator siguiendo un script

![alt text](/img/blog/generar-b2b-accionable-lista-sales-navigator.png "Captura de pantalla de listado")

El comando final se daba de esta manera:

**=C2&D2&B2&G2&E2&A2&F2**

Necesitamos una búsqueda base de Linkedin que no se modifique, podría ser:

**Linkedin.com/sales/search/people?**

Y luego agregamos los parámetros:

companysize= 

- “A” para autónomo 
- “B” para 1-10 empleados
- “C” para 11-50, etc

&titleincluded=
&keywords=
&titleTimeScope=CURRENT

Generamos un Phantom en Phantombuster de Sales Navigator Search Exports para obtener todos los perfiles posibles según esas variables.

![alt text](/img/blog/export-sales-navigator-phantom.png "Captura de pantalla de exportación de Sales Navigator")

Hecho esto, utilizamos Texau o Phantombuster para hacer una extracción de todos esos perfiles de Linkedin. 

![alt text](/img/blog/scrape-linkedin-sales-navigator.png "Captura de pantalla de Scrape de Sales Navigator")

Con los URL de Linkedin conseguidos, los importamos a One2Lead para generar 2 campañas diferentes.

![alt text](/img/blog/importar-one2lead.png "Captura de pantalla de importación en One2Lead")

Una para hacer los envíos de conexión diarios de forma 100% automática. Otra para hacer un seguimiento si no habían respondido al mensaje de la conexión.

De esta manera generamos un engagement acelerado para convertir cada vez más reuniones.

**“Hola #name#! Cómo estás? Tengo entendido que en #company# tu te encargas de mantenimiento y demás? O las decisiones las toma otra persona?”**

*Nunca está de más apelar al ego de un directivo para aumentar el reply rate.*

A medida que aceptan las invitaciones, aprovechamos el 1er grado de Linkedin para ver si encontramos un mail de la persona decisora.

Utilizamos herramientas como FindThatLead o Hunter.io para buscar todas las coincidencias. A los que daban más de 80%, los incluímos en una lista de mailing automatizada para buscar conseguir una reunión con el decisor 

![alt text](/img/blog/findthatlead-hunter-match.png "Captura de pantalla de búsqueda de perfiles de redes sociales utilizando Find That Lead")

*Nota: por cada 1000 personas de Linkedin, probablemente se encuentren 40% de mails confiables, de los cuales probablemente la mitad no sean corporativos. Es recomendable hacer muchas tandas para armar estas bases, ya que la tasa% de calificación, si es muy fina, requiere un proceso adecuado.*

Si existe esa forma de contacto, utilizamos Gmass para hacer envíos masivos simulando enviarlos desde nuestro mail, para evitar caer en Spam o promociones como si estuviésemos usando Mailchimp o herramientas similares. 

![alt text](/img/blog/gmass.png "Captura de pantalla de la aplicación Gmass")

*Nota: para cuidar el score de una casilla de mail, al principio es ideal hacer pruebas con otro mail diferente al “oficial” que vayamos a querer usar. No queremos correr el riesgo de volvernos una casilla sospechosa para cuando tengamos el workflow B2B validado.*

De esta manera generamos un multimpacto que desembocaba en gran cantidad de reuniones para un servicio super segmentado según las industrias trabajadas.

Adicionalmente, con <a href="https://zapier.com/blog/push-by-zapier-google-chrome-extension/" target="_blank">Push</a> de Zapier generamos una automatización para que la persona de ventas pudiese simular una conexión a Hubspot y gestionase los leads una vez ingresados en el sistema.