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

### Acitividad 12 P48

ReciboComunidad(**numero**, fecha, importe, NCatasral)

ReciboCompañia((**numero**, fecha, importe, NContrato, CIF)

Cuenta(**sucursal**, **control**, **numero**, saldo)





