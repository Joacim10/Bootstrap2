<template>
    <nav class="navbar navbar-expand-lg navbar-light bg-white">
        <div class="container">  
            <div class="">
                <a class="navbar-brand" href="#">KEN KATA</a>
                <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
                    <span class="navbar-toggler-icon"></span>
                </button>
            </div>

            <div class="collapse navbar-collapse" id="navbarSupportedContent">
                <form class="ml-auto mr-lg-4 form-inline my-lg-0">
                    <div class="input-group">
                    <input type="text" class="form-control" aria-label="Text input with segmented dropdown button">
                    <div class="input-group-append">
                        <button type="button" class="btn btn-outline-secondary dropdown-toggle dropdown-toggle-split" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                            Categories
                            <span class="sr-only">Toggle Dropdown</span>
                        </button>
                        <div class="dropdown-menu">
                            <a class="dropdown-item" href="#">Action</a>
                            <a class="dropdown-item" href="#">Another action</a>
                            <a class="dropdown-item" href="#">Something else here</a>
                            <div role="separator" class="dropdown-divider"></div>
                            <a class="dropdown-item" href="#">Separated link</a>
                        </div>
                    </div>
                        <button type="button" class="bg-info btn btn-outline-secondary">
                        <a href="">S</a>
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

<style>

</style>