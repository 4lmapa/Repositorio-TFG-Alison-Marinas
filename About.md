![Cover](https://github.com/4lmapa/tfg-amp_manual-repo/blob/master/Banners/banner00.jpg)

## 🌱 Presentación
 
>**_Este manual teórico-práctico introduce al diseño de productos basados en formas y estructuras bioinspiradas con Grasshopper, un editor de programación visual complementario al modelador Rhinoceros 3D._**

Los contenidos de este manual se componen de capítulos teóricos y prácticos, dividiendo el manual en dos partes claramente diferenciadas para su organización y uso.

### Parte 01. Contenidos teóricos

La **primera parte** de este manual abarca los capítulos teóricos dedicados al estudio de la biomímesis en el diseño de estructuras para el desarrollo de objetos a través de herramientas computacionales. En este estudio teórico se presenta el estado del arte del diseño bioinspirado ─donde la biomímesis se proclama como la disciplina de referencia en el estudio de las estrategias naturales para su aplicación en problemas humanos─, de los sistemas estructurales y de las últimas herramientas que ofrece el diseño computacional.

* **01 Naturaleza como modelo de diseño**
  * 011 Evolución histórica
  * 012 Principios biomiméticos en el diseño 
  * 013 Biomímesis en el diseño de estructuras 

* **02 Estructuras y sistemas estructurales**
  * 021 Clasificación de los sistemas estructurales
  * 022 Geometría de las formas estructurales 

* **03 Sistemas estructurales naturales**
  * 031 Clasificación de estructuras naturales 
  * 032 Estructuras naturales vs. estructuras artificiales

* **04 Diseño computacional**
  * 041 Terminología computacional 
  * 042 Software para el diseño de estructuras

### Parte 02. Contenidos prácticos

En la **segunda parte** de este manual se abordan seis casos prácticos consistentes en tutoriales de Grasshopper donde se introduce a la metodología de trabajo con software de programación visual. Dichos tutoriales se centran en la reproducción de tres estructuras naturales: basadas en **diagramas de Voronoi**, **tipo Gyroid** y **reticulares**. Y se aplican en otros tres tutoriales para el diseño de tres objetos: **un anillo**, **una lámpara** y **la suela de una zapatilla**, respectivamente. 
La relación entre el sistema estructural natural, los tutoriales de base y los tutoriales de aplicación se reflejan en la siguiente tabla:

nº | Estructural natural                                           | Tutorial de base | Tutorial de aplicación
:-:| :------------------------------------------------------------ | :--------------: | :--------------------:
1  | Estructuras basadas en la teselación por diagramas de Voronoi | [TB1][25]        | [TA1][26]
2  | Superficies Mínimas Triple Periódicas: Schwarz G (Gyroid)     | [TB2][27]        | [TA2][28]
3  | Estructuras reticulares                                       | [TB3][29]        | [TA3][30]

* **Estructura 1**
  * **[TB1][25] ─ Tutorial Básico 1.** Desarrollo de estructura reticular a partir de la intersección de regiones Voronoi 3D
  * **[TA1][26] ─ Tutorial Avanzado 1.** Desarrollo de anillo definido por una estructura laminar perforada a partir de regiones Voronoi 3D

* **Estructura 2**
  * **[TB2][27] ─ Tutorial Básico 2.** Desarrollo de entramado definido por la célula unitaria de una superficie Gyroid
  * **[TA2][28] ─ Tutorial Avanzado 2.** Desarrollo de lámpara con entramado superficial definido por una superficie Gyroid

* **Estructura 3**
  * **[TB3][29] ─ Tutorial Básico 3.** Desarrollo de entramado reticular puro de módulo bioinspirado
  * **[TA3][30] ─ tutorial Avanzado 3.** Desarrollo de suela de zapatilla definida por un entramado reticular de flexibilidad variable
  
---
  
![Divider 1](https://github.com/4lmapa/tfg-amp_manual-repo/blob/master/Banners/banner01.jpg)

## ⚡ Requisitos y configuraciones previas

### Programas
Los tutoriales incluidos en este manual se han desarrollado empleando los programas:
* [Rhinoceros 5 SR5](https://www.rhino3d.com/download/rhino/5/latest)
* [Grasshopper 0.9.0076](https://www.grasshopper3d.com/page/download-1) (para Rhinoceros 5)

Las versiones empleadas del *software* no son las últimas lanzadas ya que muchos de los complementos y *scripts* aún no están optimizados para Rhinoceros 6.

### Lista de complementos
Además de los mencionados programas, se hará uso de los siguientes *scripts* complementarios a Grasshopper:

Complemento       | Autor                        | Fuente Oficial 🡭              | Archivo
:---------------- | :--------------------------- | :----------------------------- | :--------:
`Cocoon`          | *[David Stasiuk][18]*        | [Bespoke Geometry][1]          | [.zip][11]
`Crystallon`      | *[Aaron Porterfield][19]*    | [Food4Rhino][2]                | [.zip][12]
`Kangaroo Physics`| *[Daniel Piker][20]*         | [Food4Rhino][3]                | [.zip][13]
`MeshEdit`        | *[[uto]-lab][21]*            | [Food4Rhino][4]                | [.zip][14]
`MeshMachine`     | *[Daniel Piker][22]*         | [Grasshopper3D][5]             | [.gha][15]
`Millipede`       | *[Panagiotis Michalatos][23]*| [Grasshopper3D][6] 🚩          | [.zip][16]
`Weaverbird`      | *[Giulio Piacentino][24]*    | [Giulio Piacentino Website][7] | [.msi][17]

:triangular_flag_on_post: 25/06/2020 ─ Debido a problemas en la [~~página web oficial~~][8] se remite al repositorio *[Millipede Backup][9]* creado por [@nickteeple][10].

---

## ▶ Instrucciones de uso

### Estructura de los tutoriales
Buscando la practicidad y la simplicidad de uso, todos los tutoriales comparten una estructura común.
Esta estructura está compuesta por:
- Una breve **descripción** del diseño que se va a realizar en el tutorial.
- Un apartado en el que se nombran los **scripts y archivos** necesarios para la elaboración del tutorial.
- Un apartado que resume el **procedimiento** seguido.
- Un apartado que explica en detalle y **paso por paso** el procedimiento.

### Acciones comunes
Tras realizar todas las **configuraciones previas** al uso de los tutoriales se describen a continuación las acciones comunes previas:
1. Ejecutar **Rhinoceros**.
2. Escribir `Grasshopper` en la línea de comandos de **Rhinoceros** para acceder a la interfaz de este.

---

![Divider 2](https://github.com/4lmapa/tfg-amp_manual-repo/blob/master/Banners/banner013.jpg)

## 📂 Bibliografía

Este manual **requiere de un nivel básico de habilidad** con Rhinoceros y Grasshopper para la realización de los tutoriales. En caso de no tener dicha formación básica, se pone a disposición la siguiente **Bibliografía** con una gran variedad de recursos para el aprendizaje de dichos programas:

* **Páginas web**

  * David Rutten. (s.f.). _Grasshopper Basics with David Rutten._ Consultado el 25 de junio de 2020. https://vimeopro.com/rhino/grasshopper-getting-started-by-david-rutten
  * Grasshopper Docs. (s.f.). _Community documentation for Grasshopper add-ons & plugins._ Consultada el 24 de junio de 2020. http://grasshopperdocs.com/
  * Grasshopper3D. (s.f.-b). _Getting started._ Consultada el 24 de junio de 2020. https://www.grasshopper3d.com/page/tutorials-1
  * McNeel Wiki. (s.f.). _Manuales de formación de Rhino 6._ Consultado el 21 de junio de 2020. https://wiki.mcneel.com/es/rhino/6/trainingguides/en
  * Rhino3D. (s.f.). _Formación._ Consultado el 21 de junio de 2020. https://www.rhino3d.com/es/tutorials

* **Libros**

  * González, S. G. y Ribé, J. T. (2016). _Grasshopper para Rhinoceros e impresión 3D._ Marcombo.
  * ModeLab. (2015). _The Grasshopper Primer. An introduction to visual programming and algorithmic modeling with Rhino and Grasshopper (3.ª ed.)._ http://grasshopperprimer.com/en/index.html
  * Paynee, A. e Issa, R. (2009). _Grasshopper Primer for Version 0.6.0007 – Spanish Edition (2.ª ed.)._ http://www.miatd.org/Contenidos/Manual%20Grasshopper_Espanol.pdf



[1]:http://www.bespokegeometry.com/2015/07/22/cocoon/
[2]:https://www.food4rhino.com/app/crystallon
[3]:https://www.food4rhino.com/app/kangaroo-physics
[4]:https://www.food4rhino.com/app/meshedit
[5]:https://www.grasshopper3d.com/profiles/blogs/meshmachine-update
[6]:https://www.grasshopper3d.com/group/millipede
[7]:http://www.giuliopiacentino.com/weaverbird/

[8]:http://www.sawapan.eu/sections/section88_Millipede/downloadF.html
[9]:https://github.com/nickteeple/millipede-backup
[10]:https://github.com/nickteeple

[11]:https://github.com/4lmapa/tfg-amp_manual-repo/blob/master/Complementos/Cocoon.zip
[12]:https://github.com/4lmapa/tfg-amp_manual-repo/blob/master/Complementos/Crystallon.zip
[13]:https://github.com/4lmapa/tfg-amp_manual-repo/blob/master/Complementos/Kangaroo.zip
[14]:https://github.com/4lmapa/tfg-amp_manual-repo/blob/master/Complementos/MeshEdit.zip
[15]:https://github.com/4lmapa/tfg-amp_manual-repo/blob/master/Complementos/MeshMachine.gha
[16]:https://github.com/4lmapa/tfg-amp_manual-repo/blob/master/Complementos/Millipede.zip
[17]:https://github.com/4lmapa/tfg-amp_manual-repo/blob/master/Complementos/Weaverbird.msi

[18]:http://www.bespokegeometry.com/about/
[19]:http://fequalsf.blogspot.com/p/about.html
[20]:https://twitter.com/kangaroophysics
[21]:https://sites.google.com/site/utotoolswiki/the-team
[22]:https://www.grasshopper3d.com/profile/DanielPiker
[23]:https://www.grasshopper3d.com/profile/PanagiotisMichalatos
[24]:http://www.giuliopiacentino.com/about/

[25]:https://github.com/4lmapa/tfg-amp_manual-repo/tree/master/Tutoriales/Tutorial%20B%C3%A1sico%201
[26]:https://github.com/4lmapa/tfg-amp_manual-repo/tree/master/Tutoriales/Tutorial%20Avanzado%201
[27]:https://github.com/4lmapa/tfg-amp_manual-repo/tree/master/Tutoriales/Tutorial%20B%C3%A1sico%202
[28]:https://github.com/4lmapa/tfg-amp_manual-repo/tree/master/Tutoriales/Tutorial%20Avanzado%202
[29]:https://github.com/4lmapa/tfg-amp_manual-repo/tree/master/Tutoriales/Tutorial%20B%C3%A1sico%203
[30]:https://github.com/4lmapa/tfg-amp_manual-repo/tree/master/Tutoriales/Tutorial%20Avanzado%203
