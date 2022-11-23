<script>
export default {
    name: 'LearnSecton'
}
</script>
<template>
    <section class="learn">
        <div class="container">
            <div class="top row align-items-center mt-5">
                <div class="col-4">
                    <p class="subtitle">Why hesitate to Register?</p>
                    <h2>Learn At Your Own <span>Pace</span></h2>
                    <p>
                        <svg xmlns="http://www.w3.org/2000/svg" width="25" height="25" fill="currentColor"
                            class="bi bi-check" viewBox="0 0 16 16">
                            <path
                                d="M10.97 4.97a.75.75 0 0 1 1.07 1.05l-3.99 4.99a.75.75 0 0 1-1.08.02L4.324 8.384a.75.75 0 1 1 1.06-1.06l2.094 2.093 3.473-4.425a.267.267 0 0 1 .02-.022z" />
                        </svg>
                        Select & customize courses to your perferences
                    </p>
                    <p>
                        <svg xmlns="http://www.w3.org/2000/svg" width="25" height="25" fill="currentColor"
                            class="bi bi-check" viewBox="0 0 16 16">
                            <path
                                d="M10.97 4.97a.75.75 0 0 1 1.07 1.05l-3.99 4.99a.75.75 0 0 1-1.08.02L4.324 8.384a.75.75 0 1 1 1.06-1.06l2.094 2.093 3.473-4.425a.267.267 0 0 1 .02-.022z" />
                        </svg>
                        Change the tutor and make arrangements
                    </p>
                    <p>
                        <svg xmlns="http://www.w3.org/2000/svg" width="25" height="25" fill="currentColor"
                            class="bi bi-check" viewBox="0 0 16 16">
                            <path
                                d="M10.97 4.97a.75.75 0 0 1 1.07 1.05l-3.99 4.99a.75.75 0 0 1-1.08.02L4.324 8.384a.75.75 0 1 1 1.06-1.06l2.094 2.093 3.473-4.425a.267.267 0 0 1 .02-.022z" />
                        </svg>
                        Participate in events to join others
                    </p>
                    <p>
                        <svg xmlns="http://www.w3.org/2000/svg" width="25" height="25" fill="currentColor"
                            class="bi bi-check" viewBox="0 0 16 16">
                            <path
                                d="M10.97 4.97a.75.75 0 0 1 1.07 1.05l-3.99 4.99a.75.75 0 0 1-1.08.02L4.324 8.384a.75.75 0 1 1 1.06-1.06l2.094 2.093 3.473-4.425a.267.267 0 0 1 .02-.022z" />
                        </svg>
                        Get the desired certificate delivered at hose
                    </p>
                    <a href="#" class="btn my_btn">Get started for free</a>
                </div>
                <div class="col-6">
                    <img class="firstImg" width="300" src="../assets/img/home-5-image-01.png" alt="">
                    <img class="secondImg" src="../assets/img/maxcoach-shape-05-150x150.png" alt="">
                    <img class="therdImg" width="330" height="300" src="../assets/img/underlay-shape-grey.svg" alt="">
                </div>
            </div>
            <div class="bottom row align-items-center ">
                <div class="col-6">
                    <div class="images">
                        <img class="firstImg" width="300" src="../assets/img/home-5-image-02.png" alt="">
                        <img class="secondImg" src="../assets/img/maxcoach-shape-07-150x150.png" alt="">
                        <img class="therdImg" src="../assets/img/maxcoach-shape-01.png" alt="">
                        <img class="forImg" width="400" src="../assets/img/underlay-shape-grey.svg" alt="">
                    </div>
                </div>
                <div class="col-4">
                    <p class="subtitle">What are you looking for?</p>
                    <h2>Learn on your <span>mobile</span> anytime!</h2>
                    <p>Save lessons for later and revise or write notes at any time and on multiple devices on your way.
                        Never interfer with activities of enjoyment or other precious moments.</p>
                    <div class="">
                        <a href="#" class="btn my_btn">Download Our App</a>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>
<style lang="scss" scoped>
@use '../assets/scss/variables' as *;

.learn {
    .subtitle {
        color: $md-dark-gray;
        text-transform: uppercase;
        font-size: 13px;
        font-weight: 500;
    }

    p {
        color: $md-dark-gray;

        svg {
            color: $md-success;
        }
    }

    h2 {
        padding-bottom: 1.5rem;

        span {
            color: $md-success;
            font-weight: 350;
        }
    }

    .my_btn {
        background-color: $md-soft-primary;
        padding: 0.5rem 2.5rem;
        color: $md-light;
        font-weight: 500;
    }

    .top {
        .col-4 {
            h2 {
                width: 70%;
            }
        }

        .col-6 {
            position: relative;
            text-align: right;

            .secondImg {
                position: relative;
                top: 80px;
                left: -60px;
            }

            .therdImg {
                position: absolute;
                top: 80px;
                left: 115px;
                z-index: -1;
            }
        }
    }

    .bottom {
        margin: 10rem 0;

        .col-6 {
            .images {
                position: relative;
                z-index: 1;
            }


            .firstImg {
                position: relative;
                left: 150px;
            }

            .secondImg {
                position: absolute;
                bottom: 20px;
                left: 62%;
                z-index: -1;
            }

            .therdImg {
                position: absolute;
                top: 35%;
                left: -12%;
            }

            .forImg {
                position: absolute;
                z-index: -1;
                top: 8%;
                left: 15px;
            }
        }
    }
}
</style>