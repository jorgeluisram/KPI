<template>
 <section>
        <b-tabs position="is-centered" class="block">
            <b-tab-item label="Tabla">
                 <b-table
                :data="arreglo"
                :bordered="true"
                :hoverable="true"
                :striped="true">
                <template scope="prop">
                        <!--  <b-table-column v-if="!isFinalStatus" abel="Eliminar">
                            <b-checkbox-button  v-model="checkedIngresosOrdinariosdelMes"
                                :native-value="prop.index"
                                type="is-danger">
                                <b-icon style="margin-left: 3px;" icon="close"></b-icon>                                                                    
                            </b-checkbox-button>   
                        </b-table-column>
                        <b-table-column v-if="!isFinalStatus"  label="Editar">
                            <b-tooltip  v-model="prop.row.canEdit" label="Editar" style="margin:5px" position="is-right">
                            <button v-if="prop.row.canEdit" class="button is-success" v-on:click="enableActualRow('IngresosOrdinariosdelMes',prop.index)">
                                <span class="icon">
                                <b-icon icon="content-save" size="is-medium"></b-icon>                                                                     
                                </span>
                            </button>
                            <button v-else class="button is-warning" v-on:click="enableActualRow('IngresosOrdinariosdelMes',prop.index)">
                                <span class="icon">
                                <b-icon icon="pencil" size="is-medium"></b-icon>                                                                    
                                </span>
                            </button>                                                                
                            </b-tooltip>
                        </b-table-column> -->
                        <b-table-column label="Mes">
                            <b-input  v-model="prop.row.Dato" type="text"></b-input>
                                                                                            
                        </b-table-column>
                        
                        <b-table-column label="Ventas">
                            <b-input  v-model="prop.row.Canti" type="text"></b-input>
                                                                                            
                        </b-table-column>
                        
                </template>
            </b-table>
       

            </b-tab-item>
            <b-tab-item label="Grafica">


            </b-tab-item>
            
        </b-tabs>

            </section>
</template>
<script>
export default {
    name:"table",
    data (){
        return{
            arreglo: [
                {Dato:"Enero",Canti:30},
                {Dato:"Febrero",Canti:40},
                {Dato:"Marzo",Canti:80},
                {Dato:"Abril",Canti:100},
                {Dato:"Mayo",Canti:150}
            ]

        }
    }
}
</script>
