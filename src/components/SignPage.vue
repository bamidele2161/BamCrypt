<template>
    <div class="user-container">
            <div class="signin d-flex" v-if="isClicked">
                <form action="#" class="signin-in-form d-flex justify-content-center align-items-center flex-column" @submit.prevent="handleSubmit()">
                    <h2 class="signin-tite">Sign In</h2>
                    <div class="input-field">
                        <i class="fas fa-envelope"></i>
                        <input type="email" placeholder="Email Address" v-model="user.email">
                    </div>
                    <div class="input-field">
                        <i class="fas fa-lock"></i>
                        <input type="password" placeholder="Password" v-model="user.password">
                    </div>
                    <input type="submit" class="btn solid">
                    <p class="social-text">Or Sign in with Social Platforms</p>
                    <div class="social-media d-flex justify-content-center">
                        <a href="" class="social-icon d-flex justify-content-center align-items-center">
                            <i class="fab fa-twitter"></i>
                        </a>
                        <a href="" class="social-icon d-flex justify-content-center align-items-center">
                            <i class="fab fa-facebook"></i>
                        </a>
                        <a href="" class="social-icon d-flex justify-content-center align-items-center">
                            <i class="fab fa-instagram"></i>
                        </a>
                        <a href="" class="social-icon d-flex justify-content-center align-items-center">
                            <i class="fab fa-google"></i>
                        </a>                        
                        <a href="" class="social-icon d-flex justify-content-center align-items-center">
                            <i class="fab fa-linkedin-in"></i>
                        </a>
                    </div>
                </form>

                <div class="panel left-panel d-flex flex-column justify-content-around align-items-end text-center">
                    <div class="content">
                        <h3 class="New">New here ?</h3>
                        <p class="direction">Click on the button below to get started, we are always ready for you.</p>
                        <button class="btn transparent" id="sign-up-btn" v-if="isClicked" @click="signUp()">Sign Up</button>
                        <img src="/undraw_personal_finance_tqcd.svg" alt="#" class="image">
                    </div>
                </div>
            </div>

            <!--SignUP-->
            <div class="signup d-flex" v-if="!isClicked">
                <form action="#" class="signin-in-form d-flex justify-content-center align-items-center flex-column" @submit.prevent="handleSubmit()">
                    <h2 class="signup-tite">Sign Up</h2>
                    <div class="input-field">
                        <i class="fas fa-user"></i>
                        <input type="text" placeholder="First Name" v-model="user.firstname">
                    </div>
                    <div class="input-field">
                        <i class="fas fa-user"></i>
                        <input type="text" placeholder="Last Name" v-model="user.lastname">
                    </div>
                    <div class="input-field">
                        <i class="fas fa-envelope"></i>
                        <input type="email" placeholder="Email Address" v-model="user.email">
                    </div>
                    <div class="input-field">
                        <i class="fas fa-lock"></i>
                        <input type="password" placeholder="Password" v-model="user.password">
                    </div>
                    <input type="submit" class="btn solid">
                    <p class="social-text">Or Sign Up with Social Platforms</p>
                    <div class="social-media d-flex justify-content-center">
                        <a href="" class="social-icon d-flex justify-content-center align-items-center">
                            <i class="fab fa-twitter"></i>
                        </a>
                        <a href="" class="social-icon d-flex justify-content-center align-items-center">
                            <i class="fab fa-facebook"></i>
                        </a>
                        <a href="" class="social-icon d-flex justify-content-center align-items-center">
                            <i class="fab fa-instagram"></i>
                        </a>
                        <a href="" class="social-icon d-flex justify-content-center align-items-center">
                            <i class="fab fa-google"></i>
                        </a>                        
                        <a href="" class="social-icon d-flex justify-content-center align-items-center">
                            <i class="fab fa-linkedin-in"></i>
                        </a>
                    </div>
                </form>

                <div class="panel right-panel d-flex flex-column justify-content-around align-items-end text-center">
                    <div class="content">
                        <h3 class="New">One of Us?</h3>
                        <p class="direction">Access your account to sell your coin.</p>
                        <button class="btn transparent" id="sign-up-btn" v-if="!isClicked" @click="signIn()">Sign In</button>
                        <img src="/undraw_mobile_login_ikmv.svg" alt="#" class="image">
                    </div>
                </div>
            </div>
    </div>
</template>

<script>
// import useVuelidate from '@vuelidate/core'
import { required, minLength, maxLength} from '@vuelidate/validators'

    export default {
        name: 'SignIn_SignUp',
        data: function() {
            return{
                isClicked: false,
                user: {
                    firstname: "",
                    lastname: "",
                    email: "",
                    password: "",
                }
            };
        },
        methods: {
            signIn: function() {
                this.isClicked = true;
            },
            signUp: function() {
                this.isClicked = false;
            },
            validations: {
                firstname: {
                    required,
                    minLength: minLength(3),
                    maxLength: maxLength(10)
                },
                lastname: {
                    required,
                    minLength: minLength(3),
                    maxLength: maxLength(10)
                },
                email: {
                    required,
                    minLength: minLength(3),
                    maxLength: maxLength(10)
                },
                password: {
                    required,
                    minLength: minLength(3),
                    maxLength: maxLength(10)
                },
            },
            handleSubmit: function() {
                console.log(this.user);
                
            }

        }
    }
</script>

<style lang="scss" scoped>

</style>