<template>
    <div>
        <div class="container" style="padding:10%">
            <h2>Contact Me</h2>
            <form action="SoucekTomas@outlook.com" method="post" enctype="text/plain">
                <div class="form-group">
                    <input type="email" class="form-control" v-model="contact.eamil" placeholder="Enter email">
                </div>
                <div class="form-group">
                    <textarea class="form-control" v-model="contact.message" rows="3" placeholder="write message"></textarea>
                </div>
            </form>
            
            <button type="button" @click="submit" class="btn btn-primary btn-lg">Contact</button>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return{
            contact:{
                email:'',
                message:''
            }
        }
    },

    methods: { 
        submit(){
            if (this.contact.email !="" && this.contact.message != ""){
                //send details to email
 
            }
            else{
                alert("Fill out all fields")
            }
            
        }

    }
}
</script>