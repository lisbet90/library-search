<template> 
    <v-row class="page">
     <Header/>
     <v-row class="page-curiosidades"> 
        <v-col cols="12" md="6" lg="4" xl="3" class="mb-5 mt-3">
            <v-card class="d-flex justify-center" flat>
                <video id="player" height="240" width="380" controls download>      
                    <source id="videoSource" src="../assets/videos/video1.mp4" type="video/mp4">                    
                </video> 
            </v-card>
        </v-col>  
        <v-col cols="12" md="6" lg="4" xl="3" class="mb-5 mt-3">
            <v-card class="d-flex justify-center" flat>
                <video id="player" height="240" width="380" controls download>      
                    <source id="videoSource" src="../assets/videos/video2.mp4" type="video/mp4">                    
                </video>
            </v-card>
        </v-col>  
        <v-col cols="12" md="6" lg="4" xl="3" class="mb-5 mt-3">
            <v-card class="d-flex justify-center" flat>
                 <video id="player" height="240" width="380" controls download>      
                    <source id="videoSource" src="../assets/videos/video3.mp4" type="video/mp4">                    
                </video>
            </v-card>
        </v-col>  
     </v-row>
    </v-row>  
</template>

<script>
import Header from '../components/Header.vue'
  export default {
    name: 'Novedades',
    components: {
      Header
    },
    data: () => ({   
      loading: false,
    }),
    created(){     
      this.loading = true  
      this.loading = false  
    },
  }
</script>
