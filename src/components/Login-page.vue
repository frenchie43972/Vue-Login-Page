<template>
    <div class="container">
        <div class="row">
            <div class="col">
                <h1 class="mt-5">Login</h1>
            </div>
            <hr>
            <form-tag @myevent="submitHandler" name="myForm" event="myevent">

                <text-input 
                    v-model="email"
                    label="Email"
                    type="email"
                    name="email"
                    required="true">            
                </text-input>

                <text-input 
                    v-model="password"
                    label="Password"
                    type="password"
                    name="password"
                    required="true">            
                </text-input>
                <hr>
                <input type="submit" class="btn btn-primary" value="Login">
            </form-tag>
        </div>
    </div>    
</template>

<script>
    import FormTag from './forms/Form-tag.vue'
    import TextInput from './forms/Text-input.vue'

    export default {
        name: 'login-page',
        components: {
            FormTag,
            TextInput,
        },
        data() {
            return {
                email: "",
                password: "",
            }
        },
        methods: {
            submitHandler() {
                console.log("submitHandler called - success");
            }
        }
    }
</script>