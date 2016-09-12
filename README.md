# Notas-Angular-2
### Curso Angular 2. Sesión 1

- HTML
	- No confundir IDs con class
	- No usar tablas para layouts
- Emmet: permite escribir HTML más rápido utilziando una especie de comandos.
  http://docs.emmet.io/
  
- Pug (antiguo Jade): preprocesador HTML, parecido a Emmet. Es algo más complicado de utilizar.

- Sass: equivalente a Pug pero asociado a CSS en lugar de HTML. Es un preprocesador de CSS. Hay dos lenguajes en Sass:
	- SASS
	- SCSS: es más fácil de entender
		- Excepciones para un elemento css
		- Pseudoselectores
		- Variables --> vienen bien sobre todo para colores
		- @mixin
		- Herencia
		- -.

- CSS: Float, flexbox | Wrapper display flex http://www.bennettfeely.com/flexplorer
	- Uso de normalizadores: los navegadores tienen un estilo determinado y lo que hacen es estandarizar los estilos de partida
		para que en todos los navegadores se tenga uno común
	- Transiciones y animaciones: en CSS3 podemos aplicar animaciones sobre las propiedades de los elementos. El 90%/95 de las veces
		se hacen con transiciones, que se diferencian de las animaciones en que éstas últimas permiten poner pasos intermedios.

	- Cambio de estado del background (SCSS):
		
	-	
		```
		<div class="box">Box</div>

		.box{
		  background:#2db34a;
		  border-radius:6px;
		  cursor:pointer;
		  height:95px;
		  line-height:95px;
		  text-align:center;
		  transition-property:background;
		  transition-duration:1s;
		  transiton-timing-function:linear;
		  width:95px;
		  &:hover{
			background: #ff7b29
		  }
		}
		```
	- 	
		```
		.box {
		  background: #2db34a;
		  border-radius: 6px;
		  cursor: pointer;
		  height: 95px;
		  line-height: 95px;
		  text-align: center;
		  transition-property: background, border-radius;
		  transition-duration: 1s;
		  transiton-timing-function: linear;
		  width: 95px;
		  &:hover {
			background: #ff7b29;
			border-radius: 50%
		  }
		}
		```
	-
	
		https://codepen.io/shayhowe/pen/Fvjnf
		https://codepen.io/shayhowe/pen/hIpFr
	
	- Tipografías navegador web. El cliente / usuario podía ver tu HTML. Propiedad font-face: Puedes decirle al navegador
		qué tipografía, indicándole el archivo, quieres que use para una determinada propiedad / elemento @font-face{
		```
		font-family:"Bitstream Vera Serif Bold";
		  src:
			url("urlquesea")
		}

		h1 {
		  font-family: "Bitstream Vera Serif Bold";
		  font-size: 3em;
		}
		```
	- Bootstrap
		http://www.getbootstrap.com/
		Los css de bootstrap vienen en lenguaje less. Si en algún momento se desea modifiar el css de nuestro proyecto, se pueden 
		hacer dos cosas: o sobreescribir el css anterior con otro archivo css o cambiar el mismo
		o modificar el css
		
- Accesibilidad.
	-Niveles en tipografía
	-Modos de alto contraste
	-Tabulación	
	W3C quick ref
