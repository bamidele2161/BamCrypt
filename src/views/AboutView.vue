<template>
  <div class="about-container">
      <div className="about-page-image">
                <div className="image-content">
                    <h1 className="content-heading">ABOUT US</h1>
                    <p className="content-paragraph">Home/About</p>
                </div>
            </div>

        <div class="feature-container d-flex flex-wrap justify-content-between">
            <div class="feature-left">
                <img src="/bitcoin-many.jpg" alt="" class="feature-image">
            </div>
            <div class="feature-right">
                <h3 class="text-uppercase font-weight-bold feature-heading">Why Choose Us</h3>
                    <h1 class="mb-4 font-weight-bold">Faster, Safe and Trusted Services</h1>
                    <p class="mb-4">Dolores lorem lorem ipsum sit et ipsum. Sadip sea amet diam dolore sed et. Sit rebum labore sit sit ut vero no sit. Et elitr stet dolor sed sit et sed ipsum et kasd ut. Erat duo eos et erat sed diam duo</p>
                    <ul class="list-inline">
                        <li><h6><i class="far fa-dot-circle mr-3"></i>Best In Industry</h6></li>
                        <li><h6><i class="far fa-dot-circle mr-3"></i>Emergency Services</h6></li>
                        <li><h6><i class="far fa-dot-circle mr-3"></i>24/7 Customer Support</h6></li>
                    </ul>
                    <router-link to="/about" class="btn btn-outline-success my-2 my-sm-0 d-flex justify-content-center align-items-center" type="submit">Learn More</router-link>
            </div>
        </div>

    <FooterComponent />
  </div>
</template>

<script>
// @ is an alias to /src
import FooterComponent from '@/components/FooterComponent.vue'

export default {
  name: 'HomeView',
  components: {
    FooterComponent
  }
}
</script>
