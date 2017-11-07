<template class="temp1">
<div class="div1">
	<header class="Calculos">
		<h1>Calculos</h1>
	</header>
	<main>
		<section class="Sec1">
			<input type="number" name="" v-motel="v1">
			<input type="number" name="" v-motel="v2">
			<input type="number" name="" v-motel=resultado>
		</section>	
		<section class="Sec1">
			<button v-on:click="limpar">C</button>
			<button v-on:click="Somar">+</button>
			<button v-on:click="menos">-</button>
			<button v-on:click="multiplicar">X</button>
			<button v-on:click="dividir">%</button>
		</section>	
	</main>
</div>
</template>

<script>
export default {
	name: 'Cal',
  	data() { 
    	return {
    	v1:0,
    	v2:0,
    	resultado:null
    	}
	}, 
  methods:{
  	calc(operador){
  		if(operador==='Somar'){
  			this.resultado= this.v1+ this.v2
  		}else if (operador==='subtrair'){
     		this.resultado= this.v1- this.v2
  		}else if (operador==='multiplicar'){
  		  this.resultado= this.v1* this.v2
  		 }else if (operador==='dividir'){
  		 	this.resultado=this.v1* this.v2
	  	}
   }
 }
 </script>

<style scoped>
.h1{
	color: blue;
}		
</style>