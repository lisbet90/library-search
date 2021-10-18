<template> 
    <v-row class="page">
     <Header/>
     <v-row class="page-curiosidades"> 
        <v-col cols="12" sm="6" class="mb-5 mt-3">
            <v-row>
                <v-col cols="12" md="5" lg="4" >
                    <v-card class="d-flex justify-center" flat>
                        <v-img
                            src="../assets/img/curiosidades/cur_1.jpeg" 
                            height="153"
                            max-width="201"
                        >
                        </v-img>
                    </v-card>
                </v-col>
                <v-col cols="12" md="5" lg="8" class="contenido d-flex align-end">                   
                    <a target="_blank" :href="curiosidades[0].url" class="title font-weight-bold info-descripcion">{{curiosidades[0].title}}</a>
                </v-col>
            </v-row>          
        </v-col>  
        <v-col cols="12" sm="6" class="mb-5 mt-3">
            <v-row>
                <v-col cols="12" md="5" lg="4">
                    <v-card class="d-flex justify-center" flat>
                        <v-img
                            src="../assets/img/curiosidades/cur_2.jpeg" 
                            height="153"
                            max-width="201"
                        >
                        </v-img>
                    </v-card>
                </v-col>
                <v-col cols="12" md="5" lg="8" class="contenido d-flex align-end">                   
                    <a target="_blank" :href="curiosidades[1].url" class="title font-weight-bold info-descripcion">{{curiosidades[1].title}}</a>
                </v-col>
            </v-row>          
        </v-col>  
        <v-col cols="12" sm="6" class="mb-5 mt-3">
            <v-row>
                <v-col cols="12" md="5" lg="4">
                    <v-card class="d-flex justify-center" flat>
                        <v-img
                            src="../assets/img/curiosidades/cur_3.jpg" 
                            height="153"
                            max-width="201"
                        >
                        </v-img>
                    </v-card>
                </v-col>
                <v-col cols="12" md="5" lg="8" class="contenido d-flex align-end">                   
                    <a target="_blank" :href="curiosidades[2].url" class="title font-weight-bold info-descripcion">{{curiosidades[2].title}}</a>
                </v-col>
            </v-row>          
        </v-col>  
        <v-col cols="12" sm="6" class="mb-5 mt-3">
            <v-row>
                <v-col cols="12" md="4">
                    <v-card class="d-flex justify-center" flat>
                        <v-img
                            src="../assets/img/curiosidades/cur_4.jpg" 
                            height="153"
                            max-width="201"
                        >
                        </v-img>
                    </v-card>
                </v-col>
                <v-col cols="12" md="8" lg="8" xl="7" class="contenido d-flex align-end">                   
                    <a target="_blank" :href="curiosidades[3].url" class="title font-weight-bold info-descripcion">{{curiosidades[3].title}}</a>
                </v-col>
            </v-row>          
        </v-col>  
        <v-col cols="12" sm="6" class="mb-5 mt-3">
            <v-row>
                <v-col cols="12" md="5" lg="4">
                    <v-card class="d-flex justify-center" flat>
                        <v-img
                            src="../assets/img/curiosidades/cur_5.jpg" 
                            height="153"
                            max-width="201"
                        >
                        </v-img>
                    </v-card>
                </v-col>
                <v-col cols="12" md="5" lg="8" class="contenido d-flex align-end">                   
                    <a target="_blank" :href="curiosidades[4].url" class="title font-weight-bold info-descripcion">{{curiosidades[4].title}}</a>
                </v-col>
            </v-row>          
        </v-col>  
        <v-col cols="12" sm="6" class="mb-5 mt-3">
            <v-row>
                <v-col cols="12" md="5" lg="4">
                    <v-card class="d-flex justify-center" flat>
                        <v-img
                            src="../assets/img/curiosidades/cur_6.jpg" 
                            height="153"
                            max-width="201"
                        >
                        </v-img>
                    </v-card>
                </v-col>
                <v-col cols="12"  md="5" lg="8" class="contenido d-flex align-end">                   
                    <a target="_blank" :href="curiosidades[5].url" class="title font-weight-bold info-descripcion">{{curiosidades[5].title}}</a>
                </v-col>
            </v-row>          
        </v-col>  
     </v-row>
    </v-row>  
</template>

<script>
import Header from '../components/Header.vue'
  export default {
    name: 'Curiosidades',
    components: {
      Header
    },
    data: () => ({   
      loading: false,
      curiosidades: [
          {
              img: "cur_1.jpeg",
              title: '10 Reflexiones de Gabriel García Márquez.',
              url:'https://www.google.com/url?sa=t&source=web&rct=j&url=https://centrogabo.org/gabo/contemos-gabo/10-reflexiones-de-gabriel-garcia-marquez-sobre-las-entrevistas-periodisticas&ved=2ahUKEwifo_Ch-9LzAhV7VzABHS5GDWIQFnoECAgQAQ&usg=AOvVaw1K_sn9vP5IsGbYPOZnl2uK',
          },
          {
              img: 'cur_2.jpeg',
              title: '14 datos curiosos que quizás no sabías sobre el mundo de la literatura.',
              url:'https://www.google.com/url?sa=t&source=web&rct=j&url=https://www.lavanguardia.com/cribeo/cultura/20200423/48346161581/14-datos-curiosos-quiza-no-sabias-sobre-mundo-literatura-libros.html%3Ffacet%3Damp&ved=2ahUKEwir2Mvd1tLzAhVkSjABHfgPCYQQFnoECAQQAQ&usg=AOvVaw2AE_9bGB9IXJIH18wPxWf5&ampcf=1',
          },
          {
              img: 'cur_3.jpg',
              title: 'Día del Libro: 17 curiosidades sobre personajes, autores y obras en el mundo.',
              url:'https://www.google.com/url?sa=t&source=web&rct=j&url=https://www.eluniverso.com/entretenimiento/2019/04/23/nota/7290401/dia-libro-17-curiosidades-sobre-personajes-autores-obras/&ved=2ahUKEwir2Mvd1tLzAhVkSjABHfgPCYQQFnoECAoQAQ&usg=AOvVaw0KxmeAaEBHcdzx2IbT3Bjo',
          },
          {
              img: 'cur_4.jpg',
              title: '10 datos que no sabías de los libros y te van a sorprender.',
              url:'https://www.google.com/url?sa=t&source=web&rct=j&url=https://libros.cienradios.com/10-datos-que-no-sabias-de-los-libros-y-te-van-a-sorprender/amp/&ved=2ahUKEwir2Mvd1tLzAhVkSjABHfgPCYQQFnoECA4QAQ&usg=AOvVaw2m5XeeQQx8ju8DayAJHGSE&ampcf=1',
          },
          {
              img: 'cur_5.jpeg',
              title: 'Isabel Allende: 10 cosas que no sabías sobre su vida y obra - Milenio.',
              url:'https://www.google.com/url?sa=t&source=web&rct=j&url=https://amp.milenio.com/cultura/literatura/isabel-allende-10-sabias-vida-obra&ved=2ahUKEwiK5-WP-9LzAhW2RDABHXbCARkQFnoECA4QAQ&usg=AOvVaw2gc1JmNseAT5MDOEXH5WYy&ampcf=1',
          },
          {
              img: 'cur_6.jpeg',
              title: 'Anécdotas y datos curiosos sobre libros y escritores / Actualidad Literaria.',
              url:'https://www.google.com/url?sa=t&source=web&rct=j&url=https://www.actualidadliteratura.com/anecdotas-datos-curiosos-libros-escritores/amp/&ved=2ahUKEwir2Mvd1tLzAhVkSjABHfgPCYQQFnoECCIQAQ&usg=AOvVaw28jWtIZtgB7ixN8MJ38l4n&ampcf=1',
          },
      ]
    }),
    created(){     
      this.loading = true  
      this.loading = false  
    },
  }
</script>
