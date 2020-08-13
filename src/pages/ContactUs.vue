<template>
    <q-page>
        <div>
        <q-img src="images/phone.jpg" :ratio="27/9">
          <div class="absolute-full text-subtitle2 flex flex-center">
            <span class="text-h3 text-weight-thin"> Contact Us </span> 
          </div>
        </q-img>
      </div>

       <div id="contact-info">
            <q-page-container class="text-body1">

                <div class="q-pa-md" style="max-width: 500px" >
                    <q-list padding>                    

                    <q-item>
                        <q-item-section avatar>
                        <q-btn fab color="primary" icon="place" />
                        </q-item-section>
                        <q-item-section> <span class="text-h5">Office Address:</span> 
                        <q-item-label caption >
                            <span class="text-body2">
                            Address Address Address Address
                            Address Address Address Address
                            </span>
                        </q-item-label>
                        </q-item-section> 
                        <q-item-section side >
                        <q-badge label="HQ" />
                        </q-item-section>                   
                    </q-item>

                    <q-item>
                        <q-item-section avatar>
                        <q-btn fab color="primary" icon="email" />
                        </q-item-section>
                        <q-item-section> <span class="text-h5">Email:</span> 
                        <q-item-label caption >
                            <span class="text-body2">
                            hi@zaphirahorganics.com 
                            </span>
                        </q-item-label>
                        </q-item-section>                    
                    </q-item>

                    <q-separator spaced inset="item" />

                    <q-item>
                        <q-item-section avatar>
                        <q-btn fab color="primary" icon="call" />
                        </q-item-section>
                        <q-item-section> <span class="text-h5">Telephone</span> 
                        <q-item-label caption >
                            <span class="text-body2">
                            +234 8022223333; <br> +234 8044445555
                            </span>
                        </q-item-label>
                        </q-item-section>                    
                    </q-item>

                    <q-separator spaced />

                    </q-list>
                </div>
            </q-page-container>
        </div>
    </q-page>
</template>

<script>
export default {
    
}
</script>
<style scoped>
    #contact-info{
        margin-left:auto;
        margin-right:auto;        
    } 

</style>