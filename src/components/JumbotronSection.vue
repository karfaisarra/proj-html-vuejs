<script>
export default {
    name: 'JumbtronSection'
}
</script>
<template>
    <section class="jumbotron py-5">
        <img src="../assets/img/jumbo-overlay.svg" alt="" class="jumbo">
        <div class="container">
            <div class="row">
                <div class="col-5 align-self-center ">
                    <div class="details w-75">
                        <h2 class="mb-4 fs-1">Complate Your Dream in JavaS Programming</h2>
                        <p class="mb-4">
                            Learn any coding program in distance and for a reasonable fee. You don't have to
                            struggle alone, you've got our assistance and help.
                        </p>
                        <a href="#" class="btn my_btn d-flex justify-content-center gap-2">
                            <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor"
                                class="bi bi-download" viewBox="0 0 16 16">
                                <path
                                    d="M.5 9.9a.5.5 0 0 1 .5.5v2.5a1 1 0 0 0 1 1h12a1 1 0 0 0 1-1v-2.5a.5.5 0 0 1 1 0v2.5a2 2 0 0 1-2 2H2a2 2 0 0 1-2-2v-2.5a.5.5 0 0 1 .5-.5z" />
                                <path
                                    d="M7.646 11.854a.5.5 0 0 0 .708 0l3-3a.5.5 0 0 0-.708-.708L8.5 10.293V1.5a.5.5 0 0 0-1 0v8.793L5.354 8.146a.5.5 0 1 0-.708.708l3 3z" />
                            </svg>
                            Download free E-book
                        </a>
                    </div>

                </div>
                <div class="col-7 text-end">
                    <img width="400" src="../assets/img/home-5-hero-image.png" alt="">
                </div>
            </div>
        </div>
    </section>


</template>
<style lang="scss" scoped>
@use '../assets/scss/variables' as *;

.jumbotron {
    background-color: $md-jubo;
    position: relative;

    .jumbo {
        width: 100%;
        position: absolute;
        bottom: 0;
        height: 60%;
        transform: rotate(180deg);
    }

    .details {

        p {
            color: $md-dark-gray;
        }
    }

    .my_btn {
        background-color: $md-soft-primary;
        color: $md-light;
        font-weight: 600;
        font-size: 11px;
        padding: 0.5rem 2rem;
        width: 220px;

        & :hover {
            background-color: $md-purple;
        }
    }

}
</style>