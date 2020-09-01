<template>
    <div class="navbar navbar-expand-md navbar-dark bg-info py-0">
        <div class="container">  
            <div class="d-flex justify-content-between w-100" id="navbarSupportedContent">
                <ul class="navbar-nav mr-auto">
                    <li class="nav-item dropdown">
                        <a class="nav-link dropdown-toggle pl-0" href="#" id="navbarDropdown" role="button" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                        ENG
                        </a>
                        <div class="dropdown-menu" aria-labelledby="navbarDropdown">
                        <a class="dropdown-item" href="#">Action</a>
                        <a class="dropdown-item" href="#">Another action</a>
                        <div class="dropdown-divider"></div>
                        <a class="dropdown-item" href="#">Something else here</a>
                        </div>
                    </li>
                    <li class="nav-item dropdown">
                        <a class="nav-link dropdown-toggle" href="#" id="navbarDropdown" role="button" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                        USD
                        </a>
                        <div class="dropdown-menu" aria-labelledby="navbarDropdown">
                        <a class="dropdown-item" href="#">Action</a>
                        <a class="dropdown-item" href="#">Another action</a>
                        <div class="dropdown-divider"></div>
                        <a class="dropdown-item" href="#">Something else here</a>
                        </div>
                    </li>
                </ul>
                <div class="my-2 my-md-0">
                    <ul class="navbar-nav">
                        <li class="nav-item active border-right">
                            <router-link class="nav-link" to="#">Newsletter <span class="sr-only">(current)</span></router-link>
                        </li>
                        <li class="nav-item border-right">
                            <router-link class="nav-link" to="#">Contact Us</router-link>
                        </li>
                        <li class="nav-item border-right">
                            <router-link class="nav-link" to="#">FAQ</router-link>
                        </li>
                        <SocialMedia/>
                    </ul>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
import SocialMedia from '@/components/socialmedia/socialmedia.vue'

export default {
    components: {
        SocialMedia
    }
}
</script>

<style>

</style>