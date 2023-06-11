<template>
    <div class="container">
        <h3 class="heading">Contact Info</h3>
        <div class="section-body">
            <p>
                This is where some information to contact me is going to go. But it isn't here yet so you
                can't contact me... haha
            </p>
            <img src="../../images/contactBG.jpg" class="contact-img">
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