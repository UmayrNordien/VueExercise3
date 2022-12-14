<template>
    <div>
        <form class="contact-container">
            <!-- <label for="fullname">Fullname</label> -->
            <input type="text" placeholder="Enter fullname . . ." v-model="fullname">
            <!-- <label for="email">Email</label> -->
            <input type="email" placeholder="Enter email . . ." v-model="email">
            <!-- <label for="age">Age</label> -->
            <input type="number" placeholder="Enter age . . ." v-model="age">
            <!-- <label for="dob">DOB</label> -->
            <input type="date" placeholder="Enter date of birth . . ." v-model="dob">
            <input type="submit" class="submit-btn" id="submit" placeholder="Submit" v-on:click.prevent="submit">
        </form>
    </div>
</template>


<script>
export default {
    methods: {
        submit() {
            alert(`${this.fullname} with the email ${this.email} at age ${this.age} was born on ${this.dob}`)
        }
    },
}
</script>


<style scoped>
.contact-container {
    display: grid;
    width: 50%;
    margin: auto;
    gap: 20px;
    margin-top:20vh;
}

.submit-btn {
    width: 25%;
    margin: auto;
    margin-bottom: 20vh;

    background-color: transparent;
}
.submit-btn:hover {
    width: 25%;
    margin: auto;
    margin-bottom: 20vh;

    background-color: white;
}
</style>