---
layout:
  title:
    visible: true
  description:
    visible: false
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
---

# Unidad 3

***

### Actividad 5 P31

Alumno( **DNI**, fechaNac, nombre, apellidos)&#x20;

Asignatura ( **codigo** , nombre , curso)&#x20;

Aula ( **clase , edificio**)&#x20;

Matricula ( **Alumno** , Asignatura¬ , nota )&#x20;

imparte ( **Asignatura,** clase , edificio)&#x20;

enseña(**Profesor** , **Asignatura** , grupo)&#x20;

Profesor ( **DNI** , nombre, apellidos, antiguedad)

***

### Actividad 6 P32

Autor ( **codigo**, nombre, apellidos, fechaNac, lugarNuc )&#x20;

Libro ( **titulo** , sinopsis, genero)&#x20;

Edicion ( **ISBN** , TITULO, nEdicion, fechEdic )&#x20;

Editorial ( **NOMBRE** , telef, web, e-mail)&#x20;

Escribe (**Autor** , **Libro**)&#x20;

Escribe ( COD\_AUTOR , TITULO\_LIBRO)

***

### Actividad 7 P43

Persona ( **DNI**, nombre, NSS, apellidos, fechaNac)

&#x20;Paciente (**DNI**)&#x20;

Enfermero ( **DNI** , sueldo)&#x20;

Medico (**DNI**, especialidad, sueldo)&#x20;

Ingreso ( **numero** , tratamiento, dolencia, fechaFin, fechaIni, paciente, medico)&#x20;

EnfCronicas(Paciente, Enfermidad)&#x20;

Alergias ( Paciente , Alergia)&#x20;

Participa (**Ingreso**, **Enfermero**)

***

### Actividad 9 P45

Espejo ( **codigo** , color , foto , precio, tipo, forma)&#x20;

Marco ( **codigo** , color , foto , precio, grosor , material )&#x20;

Union( **espejo** , **Marco** )

&#x20;Sofa ( **codigo** ,color , foto , precio, Npers , catego)

chaislongue ( **codigo** ,color , foto , precio , dimension , lado)&#x20;

Adecuado ( **sofa** , **chaislongue**)

Colchon ( **codigo**, color , foto , precio, firmeza , capa)&#x20;

&#x20;Mesa ( **codigo**, color , foto , precio , forma , altura , ampliable , material)

&#x20;Componente ( **codigo**, color , foto , precio ,descrip)&#x20;

Modulo ( **codigo**, color , foto , precio, dimensiones) &#x20;

incluir(**Modulo**, Componente¬ , altura)&#x20;

Puerta ( **codigo**, color , foto , precio, tipo)&#x20;

contener(**Puerta**, Modulo¬)

***

### Actividadd 10 P46

Persona( **DNI** , Tlf , nombre, apellidos)&#x20;

Propietario (**DNI** , Tlf , nombre, apellidos )&#x20;

Inquilino (**DNI** , Tlf , nombre, apellidos)&#x20;

Comunidad  ( **DNI**, CP, calle, numero, poblacion, provincia, vocal, presidente, administrador )&#x20;

Propiedad ( **codigo** , letra, planta , comunidad, inquilino, tipo )&#x20;

dueño ( **Propietario** , **Propiedad**¬)&#x20;

Vivienda ( **Propiedad**¬ , metros)&#x20;

Local ( **Propiedad**, Actividad , Horario )&#x20;

oficina ( **Propiedad**, Actividad , Horario )

***

### Actividad 11 P47

Hotel ( ID, tlf, nombre, dirección)

Sala ( **Hotel** , numero , capacidad)

Medios ( **sala** , **medio**)

Aloja ( **Hotel** , **participante** , fechaIN, fechaOUT)

Participante ( **código** , nombre, dirección, nacionalidad, categoria)

Bailarín (**Participante**, pareja)

Jurado (**Participante**, sueldo)

Fase ( **numero**, numeroSaldo, IDHotel, hora, dia, mes, año)

Musica ( **fessa**, **cancion**)

Compite(**Participante**, **fase** , nota)

califica( **participante** , **fase**)

***

### Acitividad 14 P49

Alumno (  **DNI** , nombre, fechaNac, nivel, letra)

tutor(**email**, nombre, telefono)

materia(**nombre**)

clase(**Nivel**, **letra**, tutor)

Profesor(**DNI**, nombre, titulacion)

hermano(**alumno1** , **alumno2**)

Responsable(**tutor**, **alumno**, relacion)

imparte(**profesor**, **nivel, letra**, **materia**)

cursa(**Materia**, **Alumno,** nota)

***

### Actividad 15 P51

Galeria(**nombre**, direccion, poblacion, provincina)

Obra( **codigo**, titulo, epoca, año, tipo, galeria, autor)

autor(**nombre**, pais,fechD, fechaN)

Mecenas(**codigo**, ciudad, pais, nombre)

Patrocina(**autor**, **mecenas**, fechF,fechaI)

Maestro(**autor1**, **autor2**)

***

### Actividad 17 P52

Alumno(**codigo**, nombre, NIF, telef)

Empleado(**codigo**, nombre, NIF, NSS)

Edicion (**ID**, fechaIN, fechaFIN, horario, lugar)

Cursa(**Alumno**, **empleado**, **edicion**)

Curso(codigo, nombre, descripcion, objetivos)

prerrequisto ( **curso1**, **curso2**, obligatorio)

Unidad( **nombre**, contenido,)

***

### Actividad 18 P54

Perfil ( **email**, foto, seco, edad, trabajo, descripcion, religion,formacion)

Aficion(**codigo**, descripcion)

practica (**perfil**, **aficion**, frecuencia)

interesa(**Perfil**, **usuario**, like)

Usuario( **NIF**, telefono, usuario, pass)

cita(**ID**, fecha, lugar)

Encuesta(**Numero**, respuestas)

***

### Actividad 19 P55

Articulo(**codigo**, imagen, precio, familia, año, estacion, oferta)

oferta(**tipo**, **cantidad**)

stock(**codigo**, color, talla, cantidad, articulo)

LineaTicket(**numero**, color, talla, cantidad, coste, ticket, Articulo)

Ticket(**codigo**, formaPago, fecha, vendedor)

vendedor(**NSS**, nombre, sueldo)

LineaFactura(**numero**, color, cantidad, talla, coste, factura, Articulo)

factura(**numero**, fecha, IVA)

Representante(**ID**, nombre, telefono, email, Empresa)

Empresa(**CIF**, firmaComercial)

***

### Actividad 20 P56

trabajador( **DNI**, nombre, telefono, sueldo, ocupacion, NSS)

Afiliado(**DNI**, nombre, telefono, numero, Email, sede, cargo)

cuenta(**numero**, saldo, IBA,)

titular(**Afiliado**, **cuenta**)

Movimiento( **numero**, tipo, cantidad, concepto, cuenta)

financiacion( **codigo**, tipo, cantidad, cuenta afiliado, trabajador)

***

### Actividad 21 P57

Trabajador( **codigo**, nombre, puesto, especialidad, NIF)

cliente( **codigo**, nombre)

Mascota(**NChip** , raza, color, edad)

progenitor(

servicio( **codigo**, precio, tipo)

atiende ( **Mascota**, **servicio**, **trabajador**, fecha, descripcion)

