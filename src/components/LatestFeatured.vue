<script>
export default {
    name: 'LatestFeatured',
    data() {
        return {
            cards: [
                {
                    img: 'course-02-480x298.jpg',
                    price: '$40.00',
                    userImg: '73ee246daf47502812ccefc84bf02898 (1).jpeg',
                    userName: 'Blanche Fields',
                    description: 'Learning to Write as a Professional Author',
                    lessons: '20 Lessons',
                    students: '50 Students'
                },
                {
                    img: 'stock-full-hd-03-480x298.jpg',
                    price: 'Free',
                    userImg: 'd0d504142acfde820eef2f11feea6253 (1).jpeg',
                    userName: 'Maggie Strickland',
                    description: 'Costumer-centric Info-Tech Strategies',
                    lessons: '24 Lessons',
                    students: '769 Students'
                },
                {
                    img: 'stock-full-hd-04-480x298.jpg',
                    price: '$19.00',
                    userImg: 'd0d504142acfde820eef2f11feea6253 (1).jpeg',
                    userName: 'Maggie Strackland',
                    description: 'Open Programming Courses for Everyone: Python',
                    lessons: '17 Lessons',
                    students: '62 Students'
                },
                {
                    img: 'stock-full-hd-06-480x298.jpg',
                    price: '$26.00',
                    userImg: '73ee246daf47502812ccefc84bf02898 (1).jpeg',
                    userName: 'Blanche Fields',
                    description: 'Academic Listening and Note-talking',
                    lessons: '14 Lessons',
                    students: '67 Students'
                },
                {
                    img: 'course-featured-image-01-480x298.jpg',
                    price: '$39.00',
                    userImg: '73ee246daf47502812ccefc84bf02898 (1).jpeg',
                    userName: 'Blanche Fields',
                    description: 'Master jQuery in a Short Period of Time',
                    lessons: '6 Lessons',
                    students: '51 Students'
                },
                {
                    img: 'stock-full-hd-05-480x298.jpg',
                    price: '$59.00',
                    userImg: '73ee246daf47502812ccefc84bf02898 (1).jpeg',
                    userName: 'Blanche Fields',
                    description: 'Introduction to Javascript for Beginners',
                    lessons: '14 Lessons',
                    students: '76 Students'
                },

            ]
        }
    },
    methods: {
        getImageUrl(url) {
            return new URL(`../assets/img/${url}`, import.meta.url).href
        }
    }
}
</script>
<template>
    <section class="latest">
        <div class="container">
            <p class="subtitle">Choose where you'd like to begin</p>
            <h2>Latest Featured <span>Courses</span></h2>
            <div class="row row-cols-lg-3 g-5">
                <div class="col" v-for="card in cards">
                    <div class="card border-0 ">
                        <div card_top>
                            <img class="card-img-top" :src="getImageUrl(card.img)" alt="">
                            <div class="price">
                                {{ card.price }}
                            </div>
                        </div>
                        <div class="card-text p-4">
                            <div class="user">
                                <img width="30" class="rounded-pill" :src="getImageUrl(card.userImg)" alt="">
                                <span>{{ card.userName }}</span>
                            </div>
                            <h5 class="w-75">{{ card.description }}</h5>
                            <div class="icons d-flex align-items-center gap-4">
                                <div class="left d-flex align-items-center">
                                    <svg xmlns="http://www.w3.org/2000/svg" width="13" height="13" fill="currentColor"
                                        class="bi bi-file-earmark-arrow-down me-1" viewBox="0 0 16 16">
                                        <path
                                            d="M8.5 6.5a.5.5 0 0 0-1 0v3.793L6.354 9.146a.5.5 0 1 0-.708.708l2 2a.5.5 0 0 0 .708 0l2-2a.5.5 0 0 0-.708-.708L8.5 10.293V6.5z" />
                                        <path
                                            d="M14 14V4.5L9.5 0H4a2 2 0 0 0-2 2v12a2 2 0 0 0 2 2h8a2 2 0 0 0 2-2zM9.5 3A1.5 1.5 0 0 0 11 4.5h2V14a1 1 0 0 1-1 1H4a1 1 0 0 1-1-1V2a1 1 0 0 1 1-1h5.5v2z" />
                                    </svg>
                                    <span>{{ card.lessons }}</span>
                                </div>
                                <div class="right d-flex align-items-center">
                                    <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor"
                                        class="bi bi-person me-1" viewBox="0 0 16 16">
                                        <path
                                            d="M8 8a3 3 0 1 0 0-6 3 3 0 0 0 0 6Zm2-3a2 2 0 1 1-4 0 2 2 0 0 1 4 0Zm4 8c0 1-1 1-1 1H3s-1 0-1-1 1-4 6-4 6 3 6 4Zm-1-.004c-.001-.246-.154-.986-.832-1.664C11.516 10.68 10.289 10 8 10c-2.29 0-3.516.68-4.168 1.332-.678.678-.83 1.418-.832 1.664h10Z" />
                                    </svg>
                                    <span>{{ card.students }}</span>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            <div class="call_to_action">
                <a href="#" class="btn my_btn">
                    View all courses
                    <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor"
                        class="bi bi-arrow-right" viewBox="0 0 16 16">
                        <path fill-rule="evenodd"
                            d="M1 8a.5.5 0 0 1 .5-.5h11.793l-3.147-3.146a.5.5 0 0 1 .708-.708l4 4a.5.5 0 0 1 0 .708l-4 4a.5.5 0 0 1-.708-.708L13.293 8.5H1.5A.5.5 0 0 1 1 8z" />
                    </svg>
                </a>
            </div>
        </div>
    </section>
</template>
<style lang="scss" scoped>
@use '../assets/scss/variables' as *;

.latest {
    background-color: #F6F6F6;
    padding-top: 3rem;

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

        span {
            color: $md-success;
            font-weight: 350;
        }
    }

    .card {
        background-color: transparent;

        .card_top {

            .card-img-top {
                position: relative;
            }
        }

        .price {
            position: absolute;
            top: 0;
            right: 0;
            background-color: $md-soft-primary;
            padding: 0.5rem 0.75rem;
            width: 90px;
            height: 40px;
            text-align: center;
            color: $md-light;
            border-radius: 0 5px 0 5px;
            font-weight: bold;
        }

        .card-text {
            .user {
                margin-bottom: 0.75rem;

                span {
                    color: $md-dark-gray;
                    padding-left: 0.5rem;
                    font-size: 13px;
                    font-weight: 500;
                }
            }

            .icons {
                margin-top: 1.5rem;
                font-size: 13px;
                color: $md-dark-gray;
                font-weight: 500;
            }
        }

        &:hover {
            background-color: $md-light;
            box-shadow: 5px 5px 5px 5px #8888880c;
            cursor: pointer;
        }
    }

    .call_to_action {
        text-align: center;
        padding: 4rem 0;

        .my_btn {
            background-color: $md-soft-primary;
            padding: 0.5rem 2.5rem;
            color: $md-light;
            font-weight: 500;

            &:hover {
                color: $md-soft-primary;
                background-color: $md-light;
            }
        }
    }
}
</style>