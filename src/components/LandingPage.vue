<template>
    <div class="landing-container">

        <div class="hero-container d-flex flex-wrap justify-content-between">
            <div class="hero-left-div d-flex flex-column">
                <h1 class="hero-heading">The World's Fastest <br/>Growing <span style="color: #030392">Crypto</span> Exchange</h1>
                <p class="hero-details">Lorem ipsum dolor, sit amet consectetur adipisicing elit. Inventore,<br /> provident ab blanditiis aliquid aut vero repudiandae repellat sint officia ratione.</p>
                <router-link id="hero-btn-lg" to="/getStarted" class="btn btn-outline-success my-2 my-sm-0 d-flex justify-content-center align-items-center" type="submit">Get Started</router-link>
            </div>
            <div class="hero-right-div d-flex justify-content-center align-items-center">
                <img src="/heroOne.svg" alt="" class="hero-image">
            </div>
        </div>

        <div class="invest-div d-flex flex-wrap justify-content-center flex-column">
            <h2 class="invest-heading text-center font-weight-bold">Invest in the Future with Confidence</h2>
            <div class="card-deck">
                <div class="card text-center p-10">
                    <i class="fa-solid fa-money-check-dollar" id="card-hero-first-icon"></i>
                    <div class="card-body">
                        <h5 class="card-title">Transaction Made Easy</h5>
                        <p class="card-text">This is a wider card with supporting text below as a natural lead-in to .</p>
                    </div>
                </div>
                <div class="card text-center p-10">
                    <i class="fa-solid fa-coins" id="card-hero-second-icon"></i>
                    <div class="card-body">
                        <h5 class="card-title">No Fear of Loss</h5>
                        <p class="card-text">This card has su</p>
                    </div>
                    
                </div>
                <div class="card text-center p-10">
                    <i class="fa-solid fa-lock" id="card-hero-third-icon"></i>
                    <div class="card-body">
                        <h5 class="card-title">Security</h5>
                        <p class="card-text">This is a wider card with supporting text below a.</p>
                    </div>
                </div>
            </div>
        </div>

        <div class="feature-container d-flex flex-wrap justify-content-between">
            <div class="feature-left">
                <img src="/bitcoin-manyO.jpg" alt="" class="feature-image">
            </div>
            <div class="feature-right">
                <h3 class="text-uppercase feature-heading">Why Choose Us</h3>
                    <h1 class="mb-4 font-weight-bold">Faster, Safe and Trusted Services</h1>
                    <p class="mb-4 dolores">Dolores lorem lorem ipsum sit et ipsum. Sadip sea amet diam dolore sed et. Sit rebum labore sit sit ut vero no sit. Et elitr stet dolor sed sit et sed ipsum et kasd ut. Erat duo eos et erat sed diam duo</p>
                    <ul class="list-inline">
                        <li><h6><i class="far fa-dot-circle mr-3"></i>Best In Industry</h6></li>
                        <li><h6><i class="far fa-dot-circle mr-3"></i>Emergency Services</h6></li>
                        <li><h6><i class="far fa-dot-circle mr-3"></i>24/7 Customer Support</h6></li>
                    </ul>
                    <router-link to="/about" class="btn btn-outline-success my-2 my-sm-0 d-flex justify-content-center align-items-center" type="submit">Learn More</router-link>
            </div>
        </div>

        <div class="confidence-container d-flex flex-wrap justify-content-between">
            <div class="confidence-left">
                <h3 class="text-uppercase confidence-heading">Trade with Confidence</h3>
                    <h1 class="mb-4 font-weight-bold">Most Secured Crypto Exchange</h1>
                    <p class="mb-4 dolores">Dolores lorem lorem ipsum sit et ipsum. Sadip sea amet diam dolore sed et. Sit rebum labore sit sit ut vero no sit. 
                        Et elitr stet dolor sed sit et sed ipsum et kasd ut. Erat duo eos et erat sed diam duo
                        Lorem ipsum dolor sit amet consectetur adipisicing elit. Quibusdam similique cupiditate repellat commodi, 
                        aliquam, et obcaecati consequuntur, 
                        natus ipsum aliquid quo assumenda velit saepe! Nobis sint rem laudantium facilis esse!
                        </p>
                    <!-- <ul class="list-inline">
                        <li><h6><i class="far fa-dot-circle mr-3"></i>Best In Industry</h6></li>
                        <li><h6><i class="far fa-dot-circle mr-3"></i>Emergency Services</h6></li>
                        <li><h6><i class="far fa-dot-circle mr-3"></i>24/7 Customer Support</h6></li>
                    </ul> -->
                    <router-link to="/about" id="confidence-btn" class="btn my-2 my-sm-0 d-flex justify-content-center align-items-center" type="submit">Learn More</router-link>
            </div>
            <div class="confidence-right">
                <img src="/bitcoin.png" alt="" class="confidence-image">
            </div>
            
        </div>
<!-- 
        <div class="news-container d-flex flex-wrap justify-content-center flex-column">
            <h2 class="news-heading text-center">Our Latest News & Articles</h2>
            <div class="card-deck">
                <div class="card text-center p-20">
                    <img class="card-img-top" src="/bitcoinTwo.jpg" alt="Card image cap">
                    <div class="card-body">
                        <h5 class="card-title">Investment in Bitcoin</h5>
                        <p class="card-text">This is a longer card with supporting text below as a natural lead-in to additional content.</p>
                    <router-link to="/about" class="btn btn-outline-success d-flex justify-content-center align-items-center" type="submit" id="re-more-btn">Read More <i class="fa-solid fa-arrow-right"></i></router-link>
                    </div>
                </div>
                <div class="card text-center p-20">
                    <img class="card-img-top" src="/ethereum.jpg" alt="Card image cap">
                    <div class="card-body">
                        <h5 class="card-title">Investment in Ethereum</h5>
                        <p class="card-text">This card has supporting text below as a natural lead-in to additional content.</p>
                    <router-link to="/about" class="btn btn-outline-success d-flex justify-content-center align-items-center" type="submit" id="re-more-btn">Read More <i class="fa-solid fa-arrow-right"></i></router-link>
                    </div>
                </div>
                <div class="card text-center d.flex flex-column align-items-center justify-content-center p-20">
                    <img class="card-img-top" src="/chart.jpg" alt="Card image cap">
                    <div class="card-body">
                        <h5 class="card-title">The Crypto Market</h5>
                        <p class="card-text">This is a wider card with supporting text below as a natural lead-in to additional content. </p>
                    <router-link to="/about" class="btn d-flex justify-content-center align-items-center" type="submit" id="re-more-btn">Read More <i class="fa-solid fa-arrow-right"></i></router-link>
                    </div>
                </div>
            </div>
        </div> -->

        <div class="faqs-container">
            <h2 class="faqs-heading text-center font-weight-bold">Frequently Asked Questions</h2>
            <p class="faqs-paragraph text-center">We know you have some questions in mind</p>
            <div class="faqs-card-container d-flex flex-column">
                <div class="question-div">
                    <div class="question-line d-flex justify-content-between font-weight-bold" >
                        <p class="question-text ">What problems do you solve ?</p>
                        <i class="fa-solid fa-angle-up" v-if="isDropped" @click="close()" id="faqs-arrow"></i>
                        <i class="fa-solid fa-angle-down" v-if="!isDropped" @click="open()" id="faqs-arrow"></i>
                    </div>
                    <p class="answer-text" v-if="isDropped">BAMCRYPT is the best cryptocurrency trading platform. Trade cypto simple, top cryptocurrency exchange platform and the best platform to buy cryptocurrency</p>
                </div>


            </div>
        </div>

    </div>
</template>

<script>
    export default {
        name: "LandingPage",
        data: function() {
            return{
                isDropped: false,
            };
        },
        methods: {
            open: function() {
                this.isDropped = true;
            },
            close: function() {
                this.isDropped = false;
            },

        }
    }
</script>

<style>

</style>