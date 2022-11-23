<script>
export default {
    name: 'EventsSection',
    data() {
        return {
            cards: [
                {
                    location: 'Texas, US',
                    descrioption: 'Storytelling Workshop',
                    day: '22',
                    month: 'NOV',
                },
                {
                    location: 'New York, US',
                    descrioption: 'Painting Art Contest 2020',
                    day: '10',
                    month: 'OCT',
                },
                {
                    location: 'Hamburg, Germany',
                    descrioption: 'International Art Fair 2020',
                    day: '23',
                    month: 'NOV',
                },
                {
                    location: 'Illinois, US',
                    descrioption: 'Street Performance: Call for Artist',
                    day: '15',
                    month: 'DEC',
                },
                {
                    location: 'Illinois, US',
                    descrioption: 'Consumer Food Safety Education Conference',
                    day: '22',
                    month: 'JUL',
                },
                {
                    location: 'Dubai, UAE',
                    descrioption: 'How meditation improve your mental health?',
                    day: '12',
                    month: 'AUG',
                },

            ]
        }
    }
}
</script>
<template>
    <section class="events">
        <div class="container my-5">
            <p class="subtitle">get in contact now</p>
            <h2>Upcoming <span>Events</span></h2>
            <div class="row row-cols-lg-2 g-4">
                <div class="col" v-for="card in cards">
                    <div class="card p-4">
                        <div class="d-flex justify-content-between">
                            <div class="left">
                                <p class="country d-flex align-items-center gap-1">
                                    <svg xmlns="http://www.w3.org/2000/svg" width="12" height="12" fill="currentColor"
                                        class="bi bi-geo-alt" viewBox="0 0 16 16">
                                        <path
                                            d="M12.166 8.94c-.524 1.062-1.234 2.12-1.96 3.07A31.493 31.493 0 0 1 8 14.58a31.481 31.481 0 0 1-2.206-2.57c-.726-.95-1.436-2.008-1.96-3.07C3.304 7.867 3 6.862 3 6a5 5 0 0 1 10 0c0 .862-.305 1.867-.834 2.94zM8 16s6-5.686 6-10A6 6 0 0 0 2 6c0 4.314 6 10 6 10z" />
                                        <path d="M8 8a2 2 0 1 1 0-4 2 2 0 0 1 0 4zm0 1a3 3 0 1 0 0-6 3 3 0 0 0 0 6z" />
                                    </svg>
                                    <span>{{ card.location }}</span>
                                </p>
                                <h5 class="">{{ card.descrioption }}</h5>
                            </div>
                            <div class="right text-center">
                                <h2>{{ card.day }}</h2>
                                <h6>{{ card.month }}</h6>
                                <a href="#" class="btn my_btn">Get ticket</a>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            <div class="call_to_action">
                <p>Excited about our envent?
                    <a href="#">
                        View all events
                        <svg xmlns="http://www.w3.org/2000/svg" width="15" height="15" fill="currentColor"
                            class="bi bi-arrow-right" viewBox="0 0 16 16">
                            <path fill-rule="evenodd"
                                d="M1 8a.5.5 0 0 1 .5-.5h11.793l-3.147-3.146a.5.5 0 0 1 .708-.708l4 4a.5.5 0 0 1 0 .708l-4 4a.5.5 0 0 1-.708-.708L13.293 8.5H1.5A.5.5 0 0 1 1 8z" />
                        </svg>
                    </a>
                </p>
            </div>
        </div>
    </section>
</template>
<style lang="scss" scoped>
@use '../assets/scss/variables' as *;

.events {
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

    .card {
        background-color: #F8F8F8;
        border: 0 solid transparent;

        .left {
            .country {

                span,
                svg {
                    color: $md-dark-gray;
                }

                span {
                    font-size: 12px;
                    font-weight: 500;
                }
            }

            h5 {
                margin-top: -10px;
            }
        }

        .right {
            h2 {
                color: $md-soft-primary;
                margin-bottom: -1px;
            }

            h6 {
                font-size: 15px;
            }

            .my_btn {
                background-color: $md-soft-primary;
                padding: 0.25rem 1.5rem;
                color: $md-light;
                font-weight: 500;
            }
        }

        &:hover {
            background-color: $md-light;
            box-shadow: 5px 5px 5px 5px #8888880c;
            border-left: 3px solid $md-soft-primary;

            .my_btn {
                background-color: $md-purple;
            }
        }
    }

    .call_to_action {
        margin-top: 5rem;
        text-align: center;
        color: $md-dark-gray;
        font-weight: 500;

        a {
            color: $md-soft-primary;
            text-decoration: underline;
            text-decoration-color: $md-dark-gray;
        }
    }
}
</style>