<script>
export default {
    name: 'BuildDream'
}
</script>
<template>
    <section class="build_dream py-5 text-center">
        <div class="container">
            <p class="text-uppercase mb-3">Start Learning Coding Languages</p>
            <h2 class="mb-5">Build Your Dream <span>TODAY</span></h2>
            <div class="row">
                <div class="col">
                    <img src="../assets/img/home-5-image-box-01.png" alt="">
                    <div class="details">
                        <h5>Idea Discussion</h5>
                        <p>Get teamed up with the specialists who work and teach coding for years at famous
                            universities.</p>
                        <h6>
                            <a href="#">
                                Start now
                                <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor"
                                    class="bi bi-arrow-right" viewBox="0 0 16 16">
                                    <path fill-rule="evenodd"
                                        d="M1 8a.5.5 0 0 1 .5-.5h11.793l-3.147-3.146a.5.5 0 0 1 .708-.708l4 4a.5.5 0 0 1 0 .708l-4 4a.5.5 0 0 1-.708-.708L13.293 8.5H1.5A.5.5 0 0 1 1 8z" />
                                </svg>
                            </a>
                        </h6>
                    </div>
                </div>
                <div class="col">
                    <img src="../assets/img/home-5-image-box-02.png" alt="">
                    <div class="details">
                        <h5>Web Development</h5>
                        <p>
                            Learn to start building a webpage from scratch. You decide you own pace, course and speed.
                        </p>
                        <h6>
                            <a href="#">
                                Start now
                                <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor"
                                    class="bi bi-arrow-right" viewBox="0 0 16 16">
                                    <path fill-rule="evenodd"
                                        d="M1 8a.5.5 0 0 1 .5-.5h11.793l-3.147-3.146a.5.5 0 0 1 .708-.708l4 4a.5.5 0 0 1 0 .708l-4 4a.5.5 0 0 1-.708-.708L13.293 8.5H1.5A.5.5 0 0 1 1 8z" />
                                </svg>
                            </a>
                        </h6>
                    </div>
                </div>
                <div class="col">
                    <img src="../assets/img/home-5-image-box-03.png" alt="">
                    <div class="details">
                        <h5>System Administration</h5>
                        <p>
                            Learn are encouraged to study the mechanism and structure of system administration.
                        </p>
                        <h6>
                            <a href="#">
                                Start now
                                <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor"
                                    class="bi bi-arrow-right" viewBox="0 0 16 16">
                                    <path fill-rule="evenodd"
                                        d="M1 8a.5.5 0 0 1 .5-.5h11.793l-3.147-3.146a.5.5 0 0 1 .708-.708l4 4a.5.5 0 0 1 0 .708l-4 4a.5.5 0 0 1-.708-.708L13.293 8.5H1.5A.5.5 0 0 1 1 8z" />
                                </svg>
                            </a>
                        </h6>
                    </div>
                </div>
                <div class="col">
                    <img src="../assets/img/home-5-image-box-04.png" alt="">
                    <div class="details">
                        <h5>Graphic Design</h5>
                        <p>
                            Have a passion for graphic and arts? Show your talents with confidence and
                            self-assertiveness.
                        </p>
                        <h6>
                            <a href="#">
                                Start now
                                <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor"
                                    class="bi bi-arrow-right" viewBox="0 0 16 16">
                                    <path fill-rule="evenodd"
                                        d="M1 8a.5.5 0 0 1 .5-.5h11.793l-3.147-3.146a.5.5 0 0 1 .708-.708l4 4a.5.5 0 0 1 0 .708l-4 4a.5.5 0 0 1-.708-.708L13.293 8.5H1.5A.5.5 0 0 1 1 8z" />
                                </svg>
                            </a>
                        </h6>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>
<style lang="scss" scoped>
@use '../assets/scss/variables' as *;

.build_dream {
    h2 {
        span {
            color: $md-success;
            font-weight: 350;
        }
    }

    p {
        color: $md-dark-gray;
    }

    p:first-child {
        font-size: 13px;
        font-weight: 500;
    }

    h6 {
        a {
            color: $md-dark-gray;
            text-decoration: none;
            font-weight: bold;
            font-size: 13px;
        }
    }
}
</style>