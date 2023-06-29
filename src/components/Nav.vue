<script setup>
import { RouterLink } from 'vue-router'
import { ref, onMounted } from 'vue';

onMounted(() => {
    const navLinks = document.querySelectorAll('.navbar-nav .nav-link');

    navLinks.forEach(link => {
        link.addEventListener('click', () => {
            const navbarCollapse = document.querySelector('.navbar-collapse');
            const isNavbarVisible = window.getComputedStyle(navbarCollapse).getPropertyValue('display') !== 'none';

            if (isNavbarVisible) {
                navbarCollapse.classList.remove('show');
            }
        });
    });
});
</script>

<template>
    <header>
        <nav class="navbar navbar-expand-lg">
            <div class="container-fluid">
                <RouterLink class="navbar-brand" to="/"><img src="../../public/JS2.jpg" alt="" width="80" height="80" />
                </RouterLink>
                <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav"
                    aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
                    <span class="navbar-toggler-icon"></span>
                </button>
                <div class="collapse navbar-collapse" id="navbarNav">
                    <ul class="navbar-nav">
                        <li class="nav-item">
                            <RouterLink class="nav-link" aria-current="page" to="/">Home
                            </RouterLink>
                        </li>
                        <!-- <li class="nav-item">
                            <RouterLink class="nav-link" to="/portfolio">Portfolio</RouterLink>
                        </li> -->
                        <li class="nav-item justify-content-end">
                            <RouterLink class="nav-link" to="/about">About</RouterLink>
                        </li>
                        <li class="nav-item justify-content-end">
                            <RouterLink class="nav-link" to="/contact">Contact</RouterLink>
                        </li>
                    </ul>
                </div>
            </div>
        </nav>
    </header>
</template>

<style scoped>
nav {
    padding: 20px 50px 15px;
    background: rgba(0, 0, 0, 0);
}

.nav-item {
    margin-left: 25px;
}
</style>