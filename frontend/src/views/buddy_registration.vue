<template>
    <section class="bg-white max-h-screen">
        <div class="lg:grid lg:grid-cols-12 mx-4">
            <section
                class="bg-blue-50 left-[6%] relative h-32 items-end lg:col-span-5 lg:h-full xl:col-span-6 hidden lg:block">
                <img alt="" :src="require('@/assets/images/home_animalshelter.png')"
                    class="absolute inset-0 my-20 mx-10 h-[90%] w-[90%] object-contain " />
            </section>

            <main
                class="flex items-center justify-center min-h-screen px-8 sm:px-[2rem] lg:col-span-7 lg:px-8 lg:py-12 xl:col-span-6">
                <div class="w-full md:w-2/3 mx-auto">
                    <div class="flex gap-x-2 items-center">
                        <RouterLink to="/">
                            <img alt="FrrySfLogo" title="Home" :src="logo" class="h-10 w-10" />
                        </RouterLink>
                        <h1 class="text-2xl font-semibold text-gray-800 ">Sign up as Buddy</h1>
                    </div>

                    <form action="#" class="mt-5 grid grid-cols-6 gap-6">
                        <div class="sm:col-span-6 md:col-span-3 ">
                            <label class="text-gray-800 text-sm mb-2 block font-semibold">First Name</label>
                            <input type="text" id="fname" v-model="firstName" 
                                :placeholder="firstNameError ? 'First Name is required' : 'First Name'"
                                :class="`w-full text-sm border border-gray-200 bg-white px-4 py-3 rounded-md text-gray-700 shadow-sm ${firstNameError ? 'border-red-500 placeholder-red-500' : ''}`"
                                required 
                                @focus="firstNameError = false" />
                        </div>
                        <div class="sm:col-span-6 md:col-span-3 ">
                            <label class="text-gray-800 text-sm mb-2 block font-semibold">Last Name</label>
                            <input type="text" id="lname" v-model="lastName" 
                                :placeholder="lastNameError ? 'Last Name is required' : 'Last Name'"
                                :class="`w-full text-sm border border-gray-200 bg-white px-4 py-3 rounded-md text-gray-700 shadow-sm ${lastNameError ? 'border-red-500 placeholder-red-500' : ''}`"
                                required 
                                @focus="lastNameError = false"/>
                        </div>
                        <div class="col-span-6">
                            <label class="text-gray-800 text-sm mb-2 block font-semibold">Username</label>
                            <input type="text" id="username" v-model="username" 
                                :placeholder="usernameError ? 'Username is required' : 'Username'"
                                :class="`w-full text-sm border border-gray-200 bg-white px-4 py-3 rounded-md text-gray-700 shadow-sm ${usernameError ? 'border-red-500 placeholder-red-500' : ''}`"
                                required 
                                @focus="usernameError = false"/>
                        </div>
                        <div class="col-span-6">
                            <label class="text-gray-800 text-sm mb-2 block font-semibold">Email</label>
                            <input type="email" id="email" v-model="email" 
                                :placeholder="emailError ? 'Email Address is required' : 'Email'"
                                :class="`w-full text-sm border border-gray-200 bg-white px-4 py-3 rounded-md text-gray-700 shadow-sm ${emailError ? 'border-red-500 placeholder-red-500' : ''}`"
                                required
                                @focus="emailError = false" />
                        </div>
                        <div class="col-span-6">
                            <passwordunhide v-model="password" :passwordError="passwordError" 
                                :placeholder="passwordError ? 'Password is required' : 'Password'" 
                                required />
                        </div>
                        <div class="col-span-6 gap-y-6 gap-x-6 field w-full grid sm:grid-flow-row md:grid-flow-col items-center">
                        <div class="">
                            <label for="bdate" class="text-gray-800 text-sm mb-2 block font-semibold">Birth-date</label>
                            <input type="date" id="bdate" v-model="birthdate" 
                                :class="`border w-full rounded-lg p-2 sm:text-sm ${birthdateError ? 'border-red-500' : ''}`"
                                required />
                        </div>
                        <div class="field items-center grid">
                            <label class="pr-2 text-gray-800 text-sm mb-2 block font-semibold">Gender</label>
                            <Dropdown v-model="gender" :genderError="genderError" 
                                @update:gender="gender = $event" 

                             />
                        </div>
                        </div>
                        <div class="text-center col-span-6">
                            <p class="text-sm text-gray-500">
                                By creating an account, you agree to our
                                <a href="#" class="text-gray-700 underline"> terms and conditions </a>
                                and
                                <a href="#" class="text-gray-700 underline">privacy policy</a>.
                            </p>
                        </div>
                        <div class="col-span-6 flex flex-col justify-center items-center gap-y-2 ">
                            <button @click.prevent="handleSignup()"
                                class="w-full bg-gray-800 text-white py-3 rounded-lg hover:bg-teal-600 transition duration-300">
                                Create an account
                            </button>

                            <p class="text-sm text-gray-500 sm:mt-0">
                                Already have an account?
                                <a href="#" @click="goBack" class="text-gray-700 underline">Log in</a>.
                            </p>
                        </div>
                    </form>
                </div>
            </main>
        </div>
    </section>
</template>

<script>
import axios from "axios";
import Dropdown from "../components/registration_dropdown.vue";
import passwordunhide from "../components/passwordHide.vue";
import { HomeIcon } from '@heroicons/vue/20/solid'

export default {
    name: 'LoginShelter',
    components: {
        Dropdown,
        passwordunhide,
        HomeIcon
    },
    data() {
        return {
            firstName: '',
            lastName: '',
            username: '',
            email: '',
            password: '',
            birthdate: '',
            gender: '',
            logo: require('@/assets/images/frrysfLOGO.png'),
            emailError: false,
            firstNameError: false,
            lastNameError: false,
            usernameError: false,
            passwordError: false,
            birthdateError: false,
            genderError: false,
        };
    },
    methods: {
        goBack() {
            this.$router.push({ name: 'login' }); // Navigate to login.vue
        },
        handleSignup() {
            // Reset error states before validation
            this.firstNameError = !this.firstName; // Set error if firstName is empty
            this.lastNameError = !this.lastName;   // Set error if lastName is empty
            this.usernameError = !this.username;   // Set error if username is empty
            this.emailError = !this.email;         // Set error if email is empty
            this.passwordError = !this.password;   // Set error if password is empty
            this.birthdateError = !this.birthdate; // Set error if birthdate is empty
            this.genderError = !this.gender;       // Set error if gender is not selected

            // Check if any errors exist
            if (this.firstNameError || this.lastNameError || this.usernameError || this.emailError || this.passwordError || this.birthdateError || this.genderError) {
                console.log("Some required fields are empty."); // Log error message
                return; // Prevent form submission if there are errors
            }
            // Proceed with form submission logic if no errors
            console.log('Form submitted successfully!');
            // Add your form submission logic here
        },
        async setUser() {
            try {
                const response = await axios.post("http://localhost:5000/buddy-registration", {
                    firstName: this.firstName,
                    lastName: this.lastName,
                    username: this.username,
                    email: this.email,
                    password: this.password,
                    birthdate: this.birthdate,
                    gender: this.gender,
                });
                console.log("response: ", response.data);
                if (response.data.success) {
                    this.navigateTo('/');
                } else {
                    console.log("ERRORRRRRRRRRRRRRRRRRRRRRR");
                }
            } catch (err) {
                console.log("An ERROR occurred: " + err);
            }
        }
    }
}
</script>
