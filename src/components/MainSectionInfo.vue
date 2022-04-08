<template>
    <section>
        <div class="my-container">
            <div class="row row-cols-3">
                <div class="col">
                    <div class="my-card bg-white">
                        <i class="fas fa-user-friends"></i>
                        <h5 class="card-title fw-bold mb-3">Human Capital</h5>
                        <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name:'indexMainSectionInfo'
}
</script>

<style  lang="scss" scoped>
section{
    background-color: #e3e7df;
    height: 50vh;
    width: 100%;
    i{
        color: #058283;
        background-color: #e3e7df;
        border-radius: 50%;
        padding: 12px 10px;
        margin-bottom: 1rem;
    }
}
</style>