<script>
export default {
    name: 'LoveUS'
}
</script>
<template>
    <section class="loveUs">
        <div class="container text-center">
            <p class="subtitle">People are praisig Maxcoach</p>
            <h2>What make they <span>love us?</span></h2>
            <div class="row row-cols-lg-3">
                <div class="col">
                    <div class="my_card">
                        <img width="150" class="rounded-pill" src="../assets/img/testimonial-avata-02.jpg" alt="">
                        <div class="body_card shadow rounded-2 p-5">
                            <p class="text">
                                I am free to learn at my own pace, follow my own schedule and choose the subject I like.
                                Great study portal for people like me
                            </p>
                            <h6>mina hollace</h6>
                            <p class="job">/ Freelancer</p>
                        </div>
                    </div>
                </div>
                <div class="col">
                    <div class="my_card">
                        <img width="150" class="rounded-pill" src="../assets/img/testimonial-avata-04.jpg" alt="">
                        <div class="body_card shadow rounded-2 p-5">
                            <p class="text">
                                MaxCoach is my best chois. Their tutors are smart and professional when dealing with
                                students.
                            </p>
                            <h6>Madley pondor</h6>
                            <p class="job">/ IT Specialist</p>
                        </div>
                    </div>
                </div>
                <div class="col">
                    <div class="my_card">
                        <img width="150" class="rounded-pill" src="../assets/img/testimonial-avata-01.jpg" alt="">
                        <div class="body_card shadow rounded-2 p-5">
                            <p class="text">
                                I am happy with their arrangement of lesson and subjects. They reflect a scientific
                                investigation.
                            </p>
                            <h6>mina hollace</h6>
                            <p class="job">/ Freelancer</p>
                        </div>
                    </div>
                </div>
            </div>
            <div class="select ">
                <p class="text-center"><span>.</span>...</p>
            </div>
            <div class="call_to_action">
                <h4>Start today for getting <span>Online Certification</span></h4>
                <h3>You can be your own guiding star with our help!</h3>
                <a href="#" class="btn my_btn">Get started now</a>
                <img class="right" src="../assets/img/maxcoach-shape-02.png" alt="">
                <img class="left" src="../assets/img/maxcoach-shape-01.png" alt="">
            </div>
        </div>
    </section>
</template>
<style lang="scss" scoped>
@use '../assets/scss/variables' as *;

.loveUs {
    background-color: #F8F8F8;
    padding: 4rem 0;

    .subtitle {
        color: $md-dark-gray;
        text-transform: uppercase;
        font-size: 13px;
        font-weight: 500;
        text-align: center;
    }

    h2 {
        padding-bottom: 1.5rem;
        text-align: center;
        margin-bottom: 2rem;

        span {
            color: $md-success;
            font-weight: 350;
        }
    }

    .my_card {
        margin-top: -5rem;
        padding: 2rem;

        //box-shadow: ;
        img {
            position: relative;
            top: 70px;
            left: 0;
        }

        .body_card {
            background-color: $md-light;
            width: 350px;
            height: 350px;


            .text {
                margin-top: 5rem;
            }

            h6 {
                text-transform: uppercase;
                margin-bottom: 1rem;
            }

            .job {
                color: $md-dark-gray;
            }

            &:hover {
                cursor: pointer;
            }

        }
    }

    .select {

        p {
            font-size: 75px;
            color: $md-pewter;
            margin-top: -5rem;
            letter-spacing: 10px;

            span {
                color: black;
                font-size: 100px;
            }
        }

        &:hover {
            cursor: pointer;
        }

    }

    .call_to_action {
        margin-top: 2rem;
        position: relative;

        h4 {
            span {
                color: $md-success;
                font-weight: 350;
            }
        }

        .my_btn {
            margin-top: 1.5rem;
            background-color: $md-soft-primary;
            padding: 0.5rem 3rem;
            color: $md-light;
            font-weight: 500;

            &:hover {
                color: $md-soft-primary;
                background-color: $md-light;
            }
        }

        .left {
            position: absolute;
            bottom: 40px;
            left: 170px;
        }

        .right {
            position: absolute;
            bottom: -20px;
            right: 150px;
        }
    }
}
</style>