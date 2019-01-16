<template>
	<nav class="navbar navbar-expand-md navbar-dark bg-dark mb-4">
	    <a class="navbar-brand" href="#">
	        Top navbar
	    </a>
	    <button aria-controls="navbarCollapse" aria-expanded="false" aria-label="Toggle navigation" class="navbar-toggler" data-target="#navbarCollapse" data-toggle="collapse" type="button">
	        <span class="navbar-toggler-icon">
	        </span>
	    </button>
	    <div class="collapse navbar-collapse" id="navbarCollapse">
	        <ul class="navbar-nav mr-auto">
	            <li class="nav-item active">
	                <router-link  class="nav-link" to="/home">
	                    Home
	                    <span class="sr-only">
	                        (current)
	                    </span>
	                </router-link>
	            </li>
	            <li class="nav-item">
	                <router-link  class="nav-link" to="/contact">
	                    Contact
	                </router-link>
	            </li>
	        </ul>
	        <form class="form-inline mt-2 mt-md-0">
	            <input aria-label="Search" class="form-control mr-sm-2" placeholder="Search" type="text">
	                <button class="btn btn-outline-success my-2 my-sm-0" type="submit">
	                    Search
	                </button>
	            </input>
	        </form>
	    </div>
	</nav>
</script>