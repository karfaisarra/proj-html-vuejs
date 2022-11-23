<script>
export default {
    name: 'BuildDream',
    data() {
        return {
            cards: [
                {
                    img: 'home-5-image-box-01',
                    title: 'Idea Discussion',
                    description: 'Get teamed up with the specialists who work and teach coding for years at famous universities.',

                },
                {
                    img: 'home-5-image-box-02',
                    title: 'Web Development',
                    description: 'Learn to start building a webpage from scratch. You decide you own pace, course and speed.'
                },
                {
                    img: 'home-5-image-box-03',
                    title: 'System Administration',
                    description: 'Learn are encouraged to study the mechanism and structure of system administration.'
                },
                {
                    img: 'home-5-image-box-04',
                    title: 'Graphic Design',
                    description: 'Have a passion for graphic and arts? Show your talents with confidence and self-assertiveness.'

                },
            ]
        }
    },
    methods: {
        getImageUrl(url) {
            return new URL(`../assets/img/${url}.png`, import.meta.url).href
        }
    }
}
</script>
<template>
    <section class="build_dream text-center">
        <div class="container">
            <p class="text-uppercase mb-3">Start Learning Coding Languages</p>
            <h2 class="mb-5">Build Your Dream <span>TODAY</span></h2>
            <div class="row pt-4">
                <div class="col" v-for="card in cards">
                    <img class="mb-4" :src="getImageUrl(card.img)" alt="">
                    <div class="details">
                        <h5 class="mb-4">{{ card.title }}</h5>
                        <p>{{ card.description }}</p>
                        <h6>
                            <a href="#" class="btn my_btn">
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
    margin: 4rem 0 7rem 0;

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

    .my_btn {
        padding: 0.5rem 4rem;

        &:hover {
            background-color: #F8F8F8;
            color: $md-soft-primary;
            padding: 0.5rem 4rem;
        }
    }
}
</style>