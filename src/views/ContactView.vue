<script setup>
import { supabase } from '../supabase';

var contactVid = ""

const fetchVideo = async () => {
    const { data: contactVidData } = supabase
        .storage
        .from('videos')
        .getPublicUrl('contact-vid.mp4')

    contactVid = contactVidData.publicUrl
}

fetchVideo()
</script>

<template>
    <div class="container">
        <video autoplay loop muted playsinline style="pointer-events: none;" id="bgVid" class="background">
            <source :src="contactVid" type="video/mp4" />
        </video>
        <div class="section-body">
            <address>
                <p>Email: gmjandkrj@gmail.com</p>
                <p>Phone: (501) 680-5817</p>
            </address>
        </div>
    </div>
</template>

<style scoped>
.container {
    display: grid;
    justify-content: center;
}

.heading,
.section-body {
    text-align: center;
    padding: 50px;
}

.contact-img {
    margin-top: 25px;
    height: 300px;
    width: 100%;
    object-fit: contain;
    border-radius: 25px;
    box-shadow: 5px 5px 5px 5px darkgray;
    animation: move-up-fade-in 3s;
}

.background {
    width: 100%;
    height: 300px;
}

@keyframes move-up-fade-in {
    0% {
        transform: translateY(25px);
        opacity: 0;
        box-shadow: 0px 0px 0px 0px darkgray;
    }

    100% {
        transform: translateY(0px);
        opacity: 1;
        box-shadow: 5px 5px 5px 5px darkgray;
    }
}
</style>