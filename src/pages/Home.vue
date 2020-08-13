<template>
    <div>
        <div>
          <q-carousel
            v-model="slid"
            swipeable
            animated
            autoplay
            infinite
            control-color="secondary"
            :navigation="navigation"
            :navigation-position="navPos"
            height="350px"
            class="bg-grey-8 text-white"
            >

            <q-carousel-slide :name="carousel.name" class="q-pa-none" v-for="carousel in topCarousel" :key="carousel.id">
                <div>
                    <q-img :src="carousel.imageUrl" height="350px"/>
                    <div class="custom-caption absolute-bottom text-white text-h5 text-weight-light">
                    {{ carousel.title }}
                    </div>
                </div>
            </q-carousel-slide>
          </q-carousel>
        </div>

<!-- Shop Stall -->
    <div class="bg-grey-4">         
        <div class="text-weight-light text-h4 text-primary text-center">
          Our Products!
        </div>

        <div class="text-grey-9 q-mb-sm q-px-md">
          We have the best organic products you'll need to keep your alive;
          <ul>
            <li>Zaphirah Oils</li>
            <li>Zaphirah Face and Body Scrub</li>
            <li>Zaphirah Soap</li>
            <li>Zaphirah Lip Balm</li>
          </ul>
        </div>         
<!-- Gift Cards -->
        <div class="row justify-center q-gutter-md">
          <q-card class="bg-grey-3" style="width: 100%; max-width: 300px;">
            <img src="images/pic1.jpg">
            <q-card-section>
              <div class="text-grey-8">
                <span class="text-weight-light text-primary text-h6"> Carrot & Orange Oil</span> <br>
                Carrot - 30ml (N800) | 70ml (N1,600) | 100ml (N2,800) <br>
                Orange - 30ml (N800) | 70ml (N1,200)
              </div>              
            </q-card-section>
            <q-card-actions align="right">
              <q-btn no-caps glossy rounded color="primary" label="Place Order" />
            </q-card-actions>
          </q-card>

          <q-card class="bg-grey-3" style="width: 100%; max-width: 300px;">
            <img src="images/pic3.jpg">
            <q-card-section>
              <div class="text-grey-8">
                <span class="text-weight-light text-primary text-h6"> Neem & Lemon Oil</span> <br>
                Neem - 70ml (N1,600) | 100ml (N2,800) <br>
                Lemon - 30ml (N1,200)
              </div>              
            </q-card-section>
            <q-card-actions align="right">
              <q-btn no-caps glossy rounded color="primary" label="Place Order" />
            </q-card-actions>
          </q-card> 

          <q-card class="bg-grey-3" style="width: 100%; max-width: 300px;">
            <img src="images/pic4.jpg">
            <q-card-section>
              <div class="text-grey-8">
                <span class="text-weight-light text-primary text-h6"> Rose & Coconut Oil</span> <br>
                Rosemary - 30ml (N1,200) <br>
                Coconut - 70ml (N1,600) | 100ml (N2,800)
              </div>              
            </q-card-section>
            <q-card-actions align="right">
              <q-btn no-caps glossy rounded color="primary" label="Place Order" />
            </q-card-actions>
          </q-card> 

          <q-card class="bg-grey-3" style="width: 100%; max-width: 300px;">
            <img src="images/pic2.jpg">
            <q-card-section>
              <div class="text-grey-8">
                <span class="text-weight-light text-primary text-h6"> Moringa & Avocado Oil </span> <br>
                Moringa - 30ml (N1,200) <br>
                Avocado - 70ml (N1,600) | 100ml (N2,800) 
              </div>              
            </q-card-section>
            <q-card-actions align="right">
              <q-btn no-caps glossy rounded color="primary" label="Place Order" />
            </q-card-actions>
          </q-card>                    
        </div>

<!-- Shipping -->
        <div class="text-center q-pa-md">
          <span class="text-weight-light text-primary text-h6">Shipping Information</span> <br>
          Thank you for shopping with us! <br>  
          All shipments will reach buyer in no less than 3days.
          Please fill in address correctly in appropriate field with 
          functional phone numbers to in the payment form.
        </div>
     
    </div>  
  </div>
</template>

<script>

export default {

  data () {
    return {    
    // for Carousel
      slid: 'moonlove',
      navigation: true,
      navPos: 'bottom',
      slide: 1,

      topCarousel: [
        {
          id: '1',
          name: 'moonlove',
          imageUrl: '/images/pic5.jpg',
          title: 'Glam & Glow',
        },
        {
          id: '2',
          name: 'lovecircle',
          imageUrl: '/images/pic7.jpg',
          title: 'Be Natural',
        },
        {
          id: '3',
          name: 'lovelove',
          imageUrl: '/images/pic6.jpg',
          title: 'Be Authentic',
        },
        {
          id: '4',
          name: 'loveRing',
          imageUrl: '/images/pic8.jpg',
          title: 'Be Beautiful',
        },                         
      ],      
    }
  }

}
</script>

<style scoped>

.custom-caption{
    bottom: 50px;
    text-align: center;
    padding: 5px;
    background-color: rgba(0, 0, 0, .3);
}

.radius{
  border-radius: 15px 0px 15px 0px;
  max-width: 350px;
}


/* .ruban{
    font-family:'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
} */
</style>
