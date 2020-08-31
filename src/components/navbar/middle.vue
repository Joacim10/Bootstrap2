<template>
    <nav class="navbar navbar-expand-lg navbar-light bg-white my-3">
        <div class="container">  
            <div class="">
                <a class="navbar-brand" href="#"><img src="../../assets/logo.png" alt="picture"></a>
                <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
                    <span class="navbar-toggler-icon"></span>
                </button>
            </div>

            <div class="collapse navbar-collapse" id="navbarSupportedContent">
                <form class="ml-auto mr-lg-4 form-inline my-lg-0 rounded">
                    <div class="input-group">
                    <input id="main-search" type="text" class="form-control outline-grey rounded-left" aria-label="Text input with segmented dropdown button" placeholder="Search products...">
                    <div class="input-group-append">
                        <button type="button" class="btn bg-white outline-grey dropdown-toggle-split" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                            Categories <i class="fas fa-chevron-down"></i>
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


                <div class="my-0 my-lg-0">
                    <ul class="navbar-nav">
                        <li class="nav-item active">
                            <a class="nav-link" href="#">
                                <i class="far fa-user"></i>
                                My Account 
                            </a>
                        </li>
                        <li class="nav-item active">
                            <a class="nav-link" href="#">
                                <i class="far fa-heart"></i>
                            </a>
                        </li>
                        <li class="nav-item active">
                            <a class="nav-link" href="#">
                                <i class="fas fa-random"></i>
                                <span class="badge badge-pill badge-info">0</span>
                            </a>
                        </li>
                        <li class="nav-item active">
                            <a class="nav-link" href="#">
                                <i class="fas fa-shopping-bag"></i>
                                <span class="badge badge-pill badge-info">0</span>
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
    width: 400px;
}


</style>