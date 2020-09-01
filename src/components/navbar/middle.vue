<template>
    <nav class="navbar navbar-expand-lg navbar-light bg-white mt-3 mb-lg-3">
        <div class="container d-flex justify-content-between">  
            <a class="navbar-brand" href="#"><img src="../../assets/logo.png" alt="picture"></a>

            <form class="form-inline my-lg-0 rounded">
                <div class="input-group">
                    <input id="main-search" type="text" class="d-none d-md-block form-control outline-grey rounded-left" aria-label="Text input with segmented dropdown button" placeholder="Search Products...">
                    <input id="main-search" type="text" class="d-md-none form-control outline-grey rounded-left" aria-label="Text input with segmented dropdown button" placeholder="Search...">
                    <div class="input-group-append">
                        <button type="button" class="btn bg-white outline-grey dropdown-toggle-split d-none d-md-inline-block" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                            <span>Categories</span><i class="fas fa-chevron-down"></i>
                            <span class="sr-only">Toggle Dropdown</span>
                        </button>
                        <div class="dropdown-menu dropdown-menu-right">
                            <a class="dropdown-item" href="#">Action</a>
                            <a class="dropdown-item" href="#">Another action</a>
                            <a class="dropdown-item" href="#">Something else here</a>
                            <div role="separator" class="dropdown-divider"></div>
                            <a class="dropdown-item" href="#">Separated link</a>
                        </div>
                    </div>
                    <button type="button" class="bg-info btn btn-outline-none rounded-right">
                    <a href="#"><i class="fas fa-search"></i></a>
                    <span class="sr-only">Search</span>
                    </button>
                </div>
            </form>

            <button id="navbar-toggler" class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>

            <div class="collapse navbar-collapse" id="navbarSupportedContent">
                <div class="my-0">
                    <ul class="navbar-nav flex-row justify-content-end">
                        <li class="pl-2 pl-lg-0 nav-item active">
                            <a class="nav-link" href="#">
                                <i class="far fa-user"></i>
                                My Account 
                            </a>
                        </li>
                        <li class="pl-2 pl-lg-0 nav-item active">
                            <a class="nav-link" href="#">
                                <i class="far fa-heart"></i>
                            </a>
                        </li>
                        <li class="pl-2 pl-lg-0 nav-item active">
                            <a class="nav-link" href="#">
                                <i class="fas fa-random"><span class="badge badge-pill badge-info">0</span></i>
                            </a>
                        </li>
                        <li class="pl-2 pl-lg-0 nav-item active">
                            <a class="nav-link" href="#">
                                <i class="fas fa-shopping-bag"><span class="badge badge-pill badge-info">0</span></i>
                                $0.00
                            </a>
                        </li>

                    </ul>
                </div>
            </div>
        </div>
    </nav>

</template>

<script>
export default {

}
</script>

<style scoped>
.rounded-left {
    border-radius:  50px 0 0 50px !important;
}

.rounded-right {
    border-radius:  0 50px 50px 0 !important;
}

#main-search {
    width: 120px;
}

form {
    margin-bottom: 0.5rem;
    margin-top: 0.5rem;
}

.navbar { 
    padding-top: 0;
    padding-bottom: 0;
}

@media screen and (min-width: 768px) {
    #main-search {
        width: 250px;
    }

    .navbar { 
    padding-top: 0.5rem;
    padding-bottom: 0.5rem;
}
}

@media screen and (min-width: 1200px) {
    #main-search {
        width: 400px;
    }
}

#navbar-toggler{
    margin-left: auto;
}

@media screen and (min-width: 411px) {
    #navbar-toggler{
        margin-left: 0;
    }
}

.navbar-brand {
    margin-right: 0;
}

#navbarSupportedContent {
    flex-grow: 0;
}

.badge {
    position: absolute;
    top: -7px;
    z-index: +1;
    left: 9px;
    font-size: 0.5rem;
}

.nav-link > i {
    position: relative;
}

</style>