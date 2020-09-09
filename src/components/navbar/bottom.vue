<template>
    <nav class="navbar navbar-expand-lg outline-grey navbar-light bg-white py-0">
        <div class="container">  
            <div class="collapse navbar-collapse" id="navbarSupportedContent">
                <ul class="navbar-nav mr-lg-auto flex-sm-row justify-content-between">
                    <li class="d-none d-lg-inline-block nav-item">
                        <div class="dropdown">
                        <button class="btn btn-info mr-lg-3" type="button" id="dropdownMenuButton" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                            <i class="fas fa-bars"></i>
                            Browse Categories<i class="fas fa-chevron-down"></i>
                        </button>
                        <div class="dropdown-menu dropdown-menu-right" aria-labelledby="dropdownMenuButton">
                            <a class="dropdown-item" href="#">Women</a>
                            <a class="dropdown-item" href="#">Men</a>
                            <a class="dropdown-item" href="#">Kids</a>
                        </div>
                        </div>                    
                    </li>
                    <li class="nav-item active">
                        <router-link class="nav-link" to="/">Home <span class="sr-only">(current)</span></router-link>
                    </li>
                    <li class="nav-item dropdown">
                        <a class="nav-link" href="#" id="navbarDropdown" role="button" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                        Shop<i class="fas fa-chevron-down"></i>
                        </a>
                        <div class="dropdown-menu dropdown-menu-right" aria-labelledby="navbarDropdown">
                        <router-link class="dropdown-item" to="shop">Shop</router-link>
                        <div class="dropdown-divider"></div>
                        <a class="dropdown-item" href="#">Something else here</a>
                        </div>
                    </li>
                    <li class="nav-item dropdown">
                        <a class="nav-link" href="#" id="navbarDropdown" role="button" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                        Products<i class="fas fa-chevron-down"></i>
                        </a>
                        <div class="dropdown-menu dropdown-menu-right" aria-labelledby="navbarDropdown">
                        <router-link class="dropdown-item" to="products">Products</router-link>
                        <div class="dropdown-divider"></div>
                        </div>
                    </li>
                    <li class="nav-item dropdown">
                        <a class="nav-link" href="#" id="navbarDropdown" role="button" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                        Category<i class="fas fa-chevron-down"></i>
                        </a>
                        <div class="dropdown-menu dropdown-menu-right" aria-labelledby="navbarDropdown">
                        <a class="dropdown-item" href="#">Women</a>
                        <a class="dropdown-item" href="#">Men</a>
                        <a class="dropdown-item" href="#">Kids</a>
                        </div>
                    </li>
                    <li class="nav-item dropdown">
                        <a class="nav-link" href="#" id="navbarDropdown" role="button" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                        Pages<i class="fas fa-chevron-down"></i>
                        </a>
                        <div class="dropdown-menu dropdown-menu-right" aria-labelledby="navbarDropdown">
                        <a class="dropdown-item" href="#">My Account</a>
                        <a class="dropdown-item" href="#">Shopping Cart</a>
                        <a class="dropdown-item" href="#">Wishlist</a>
                        <a class="dropdown-item" href="#">Compare</a>
                        </div>
                    </li>
                    <li class="nav-item active">
                        <a class="nav-link" href="#">Blog<span class="sr-only">(current)</span></a>
                    </li>
                </ul>
                <button class="d-none d-lg-inline-block btn btn-info ml-auto">
                    SPECIAL OFFER
                </button>
            </div>
        </div>
    </nav>
</template>

<script>
export default {

}
</script>

<style scoped>

.nav-link {
    font-size: 18px;
}

.dropdown-menu {
    position: absolute !important;
}

.nav-item{
    text-align: right;
}


</style>