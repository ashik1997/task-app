<template>
    <nav class="navbar navbar-expand-lg navbar-light bg-light border-bottom">
        <div class="container py-2">
            <a href="#" @click.prevent="$router.push('/')" class="navbar-brand">
                <span>To Do </span>
                <strong>List</strong>
            </a>
            <button
                class="navbar-toggler"
                type="button"
                data-bs-toggle="collapse"
                data-bs-target="#navbarNav"
                aria-controls="navbarNav"
                aria-expanded="false"
                aria-label="Toggle navigation"
            >
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarNav">
                <ul class="navbar-nav">
                    <li class="nav-item">
                        <router-link :to="{ name: 'tasks' }" class="nav-link">Tasks</router-link>
                         <!-- <a href="#" class="nav-link" @click.prevent="$router.push('/tasks')">Tasks</a> -->
                    </li>
                    <li class="nav-item">
                        <router-link :to="{ name: 'summary' }" class="nav-link">Summary</router-link>
                    </li>
                </ul>
                <ul class="navbar-nav ms-auto">
                    <li class="nav-item">
                        <router-link :to="{ name: 'login' }" class="btn btn-outline-secondary ms-2"
                            >Login</router-link
                        >
                    </li>
                    <li class="nav-item">
                        <router-link :to="{ name: 'register' }" class="btn btn-danger ms-2">Register</router-link>
                    </li>
                    <li class="nav-item">
                        <a href="#" class="btn btn-outline-secondary ms-2"
                            >Logout</a
                        >
                    </li>
                </ul>
            </div>

        </div>
    </nav>
</template>
<style scoped>
.nav-link.active {
    color: rgba(168, 37, 37, 0.9);
}
</style>