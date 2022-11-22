<script>
export default {
    name: 'SatisticalSection'
}
</script>
<template>
    <section class="statistical py-5">
        <div class="container">
            <div class="row">
                <div class="col">
                    <h2>1.926</h2>
                    <p>Finished sessions</p>
                </div>
                <div class="col">
                    <h2>3.092+</h2>
                    <p>Enrolled learners</p>
                </div>
                <div class="col">
                    <h2>200</h2>
                    <p>Online instructors</p>
                </div>
                <div class="col">
                    <h2>100%</h2>
                    <p>Satisfaction Rate</p>
                </div>
            </div>
        </div>
    </section>
</template>
<style lang="scss" scoped>
@use '../assets/scss/variables' as *;

.statistical {
    margin: 2rem 0;
    background-color: #FAF8F6;


    .col {
        text-align: center;

        h2 {
            color: $md-soft-primary;
            font-weight: bold;
        }

        p {
            text-transform: uppercase;
            font-weight: 500;
            font-size: 13px
        }
    }
}
</style>