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

# Unidad 2

***

### Actividad 10 P50 U2

<figure><img src="../../.gitbook/assets/image (35).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (36).png" alt=""><figcaption></figcaption></figure>

{% code fullWidth="true" %}
```html
<!DOCTYPE html>
<html>
	<head>
		<title> Tablas </title>
	</head>
	<body>
		<table border>
			<tr ALIGN = CENTER><td colspan = 6>Ciclos Formativos</td></tr>
			<tr ALIGN = CENTER><td colspan = 2>DAM</td><td colspan = 2>ASIR</td><td colspan = 2>DAW</td></tr>
			<tr ALIGN = CENTER><td>Primero</td><td>Segundo</td><td>Primero</td><td>Segundo</td><td>Primero</td><td>Segundo</td></tr>
			<tr><td>SSII</td><td>Interfaces</td><td>-</td><td>-</td><td>-</td><td>-</td></tr>
			<tr><td>BBDD</td><td>Multimedia</td><td>-</td><td>-</td><td>-</td><td>-</td></tr>
			<tr><td>Programacion</td><td>Servicios y Procesos</td><td>-</td><td>-</td><td>-</td><td>-</td></tr>
			<tr><td>Marcas</td><td>Gestion</td><td>-</td><td>-</td><td>-</td><td>-</td></tr>
			<tr><td>Entornos</td><td>Empresa</td><td>-</td><td>-</td><td>-</td><td>-</td></tr>
			<tr><td>Fol</td><td>Practicas</td><td>-</td><td>-</td><td>-</td><td>-</td></tr>
			
		</table>
		
		<table border>
			<tr><th rowspan  = 2, colspan = 2> </th><th colspan = 2>SEXO</th></tr>
			<tr><td>Hombres</td><td>Mujeres</td></tr>
			<tr><td rowspan = 2>Media</td><td>Altura</td><td>1.9</td><td>85</td></tr>
			<tr><td>Peso</td><td>1.7</td><td>60</td></tr>
		</table>
		
		<table cellpadding = 10 cellspacing = 0 border = 2>
			<caption ALIGN=top><b>Tabla 1.</b> <i>Primeras fases del ciclo de vida Software</i></caption>
			<tr ALIGN = CENTER>
				<td rowspan = 3>ANALISIS</td>
				<td>Tipos de requistos</td>
				<td>
					<ul>
						<li>Funcionales</li>
						<li>No funcionales</li>
					</ul>
				</td>
				<td rowspan = 3>Diseñoo</td>
				<td>Estructurado</td>
				<td>
					<ul>
						<li>Datos</li>
						<li>Arquitetctura</li>
						<li>interfaz</li>
						<li>Procedimental</li>
					</ul>
				</td>
			</tr>
			<tr ALIGN = CENTER>
				<td>Obtencion</td>
				<td>
					<ul>
						<li>Entrevistas</li>
						<li>BrainStorming</li>
						<li>Prototipos</li>
						<li>Casos de uso</li>
					</ul>
				</td>
				<td rowspan = 2>Orientado a Objetos</td>
				<td rowspan = 2>
					<ul>
						<li>Subsistema</li>
						<li>Clases y Objetos</li>
						<li>Mensajes</li>
						<li>Responsabilidades</li>
					</ul>
				</td>
			</tr>
			<tr ALIGN = CENTER>
				<td colspan = 2> ERS </td>
			</tr>
		</table>
	</body>




</html>
```
{% endcode %}

### Actividad 12 P62 U2

<figure><img src="../../.gitbook/assets/image (34).png" alt=""><figcaption></figcaption></figure>

{% code fullWidth="true" %}
```html
<html>
	<head>
		<title>Game of thrones</title>
		</head>
	<body>
		<! -- https://www.image-map.net/ --> 
		<p> Mapa de Game of thrones</p>
		<img src="https://i.pinimg.com/736x/ab/33/59/ab33593e3cd987a2e877c0a36da17689.jpg"
			alt="Mapa" usemap="#SSmap">
		
		<map name="SSmap">
			<area shape="circle" coords="300,256,226" alt="House Stark" href="#housestark">
			<area shape="rect" coords="286,454,516,582" alt="House Arryn" href="#housearryn">
			<area shape="poly" coords="169,565,226,564,262,661,201,743,111,763" alt="House Lannister" href="#houselannister">
			<area shape="poly" coords="223,570,261,655,307,663,387,653,428,634,432,622,242,557,233,567" alt="House Tully" href="#housetully">
			<area shape="poly" coords="303,667,484,629,496,741,350,741" alt="House Targaryen" href="#housetargaryen">
			<area shape="poly" coords="159,970,373,764,271,667,176,766,116,767,91,919" alt="House Tyrell" href="#housetyrell">
			<area shape="poly" coords="277,868,359,874,536,903,473,1003,208,995,223,904" alt="House Martell" href="#housemartell">
			<area shape="poly" coords="384,754,360,801,310,821,304,854,348,861,393,859,485,870,519,757" alt="House baratheon" href="#housebaratheon">
		</map>
		
		<a name ="housestark">
			<p><b>House Stark</b></p>
			<p> La Casa Stark de Invernalia es una casa noble del Norte. 
				Su asentamiento es Invernalia. Durante siglos, fue la casa principal del Norte y su linaje se extiende hasta los Primeros Hombres, 
				gobernando el Norte como reyes por derecho propio. Su emblema es un lobo huargo de cenizo corriendo sobre campo de plata.[1] Su lema es Se acerca el Invierno.
				Su mandoble ancestral de acero valyrio se llamaba Hielo.</p>
			
		</a>
		<a name ="housearryn">
			<p><b>House Arryn</b></p>
			<p> La Casa Arryn del Nido de Águilas es la casa principal del Valle de Arryn y las Montañas de la Luna. 
				Su asentamiento principal es el Nido de Águilas, pero tienen muchos otros asentamientos menores.
				Su linaje se extiende hasta la antigua nación de los Ándalos que invadió Poniente.
				Su emblema es una luna creciente y un halcón de plata en campo de cielo.
				Su lema es Tan Alto como el Honor.</p>
			
		</a>
		<a name ="houselannister">
			<p><b>House Lannister</b></p>
			<p>La Casa Lannister de Roca Casterly es la principal casa noble de las Tierras del Oeste.
			Su asentamiento es Roca Casterly. Su emblema es un león rampante de oro sobre campo de gules.
			Su lema es ¡Oye mi Rugido!, aunque su lema no oficial,
			Un Lannister siempre paga sus deudas, es más conocido.[3][4]</p>
		</a>
		<a name ="housetully">
			<p><b>House Tully</b></p>
			<p>La Casa Tully de Aguasdulces fue la casa principal de las Tierras de los Ríos.
			Gobernaron la región como Señores Supremos del Tridente hasta la Guerra de los Cinco Reyes,
			tras la cual fueron despojados de sus títulos y tierras por rebelarse contra el Trono de Hierro.
			Su asentamiento fue, hasta 300 d.C., Aguasdulces.
			Su linaje se extiende desde la Edad de los Héroes como Señores de Aguasdulces. Su emblema es una trucha de plata, saltando sobre campo ondulado de azur y gules.
			Su lema es Familia, Deber, Honor.</p>
		</a>
		<a name ="housearryn">
			<p><b>House Arryn</b></p>
			<p></p>
		</a>
		<a name ="housearryn">
			<p><b>House Arryn</b></p>
			<p></p>
		</a>
		<a name ="housearryn">
			<p><b>House Arryn</b></p>
			<p></p>
		</a>
		<a name ="housearryn">
			<p><b>House Arryn</b></p>
			<p></p>
		</a>
	</body>
</html>
```
{% endcode %}

### Actividad 13 P73 U2

<figure><img src="../../.gitbook/assets/image (33).png" alt=""><figcaption></figcaption></figure>

{% code fullWidth="true" %}
```html
<html>
	<head>
		<title>Actividad 13 P73</title>
	</head>
	
	<body>
		<h1>RESERVA DE HOTELES</h1>
		<fieldset>
			<legend>FORMULARIO DE RESERVA</legend><br>
			<form action="reception.html" method="post" enctype="multipart/form-data">
				<table cellpadding=5 width=100%>
					<tr><td colspan="2"><strong>>Paso 1. Identidicaci&oacute;n</strong></td></tr>
					<tr>
						<td><fieldset>
							<legend>Datos del Cliente</legend><br>
							<label for="mail">Correo electro&oacute;nico:</label><br>
							<input type="email" id="mail" size="30" maxlength="40"><br>
							<label for="pass">Contrase&ntilde;a:</label><br>
							<input type="password" id="pass" size="30" maxlength="20"><br>
							(Longitud m&iacute;nima 6 caracteres)
							</fieldset></td>
						<td width="50%">
							<fieldset>
							<legend>Datos Bancarios</legend><br>
							<label for="entidad">Nombre de la entidad</label><br>
							<input type="text" id="entidad" size="40"><br>
							<label for="num">Numero de cuenta</label><br>
							<input type="text" id="num" size="40"><br>
							</fieldset>
						</td>
					</tr>	
					<tr><td colspan="2"><strong>>Paso 2. Datos de la Reserva</strong></td></tr>
					<tr>
						<td><fieldset>
							<legend>Datos de la habitacion</legend><br>
							<select id="habitacion" name="habitacion" multiple="si" size=7>
								<optgroup label="Habitaciones">
									<option value="H001" selected="selected">H001 habitacion individual</option>
									<option value="H002" >H001 habitacion Doble</option>
									<option value="H003" >H001 habitacion Deluxe</option>
								</optgroup>
								<optgroup label="Extras">
									<option value="EX001" selected="selected">EX001 Parking</option>
									<option value="EX002">EX002 WIFI</option>
									<option value="EX003">EX003 SPA</option>
									<option value="EX004">EX004 Gimnasio</option>
								</optgroup>
							</select>
						</fieldset></td>
						<td><fieldset>
							<legend>Informacion de inter&eacute;s</legend><br> Otras peticiones<br>
							<textarea rows=6 cols=60>Escriba sus comentarios</textarea><br>
							<input type="checkbox" id="publi" value="si" checked>
							<label for="publi">Acepto recibir informacion publicitaria</label>
						</fieldset></td>
					</tr>
					
					<tr>
						<td><fieldset>
							<legend>Motivo del viaje</legend><br>
							<input type="radio" id="ocio" name="tipo" checked>
							<label for="ocio">Ocio/Turismo/Vacaciones</label><br>
							<input type="radio" id="trabajo" name="tipo">
							<label for="trabajo">Estudio/Trabajo</label><br>
							<input type="radio" id="familia" name="tipo">
							<label for="familia">Familia/Amigos</label><br>
						</fieldset></td>
						
						<td><fieldset>
							<legend>Regimen de alojamiento</legend><br>
							<select name="nivel">
								<option>Todo Incluido</option>
								<option>Pensi&oacute;n Completa</option>
								<option>Media Pensi&oacute;n</option>
								<option>Desayuno</option>
								<option selected>N/A</option>
							</select><br>
						</fieldset></td>
						<td>
						<button type="submit" style='width:130px;'>Enviar Pedido</button>
						<button type="reset" style='width:130px;'>Vaciar Formulario</button>
						</td>
					</tr>
				</table>
			</form>
		</fieldset>
	</body>
</html>
```
{% endcode %}
