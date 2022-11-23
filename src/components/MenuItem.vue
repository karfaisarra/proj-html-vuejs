<script>
export default {
    name: 'MenuItem',
    data() {
        return {
            menuEl: [
                {
                    link: '#',
                    text: 'Home'
                },
                {
                    link: '#',
                    text: 'Pages'
                },
                {
                    link: '#',
                    text: 'Courses'
                },
                {
                    link: '#',
                    text: 'Features'
                },
                {
                    link: '#',
                    text: 'Blog'
                },
                {
                    link: '#',
                    text: 'Shop'
                },
            ],
            index: 0,
        }
    },
    methods: {
        selectMenuItem(i) {
            //console.log('ho cliccato');
            this.index = i
            //console.log(this.index);
        }
    }
}

</script>
<template>
    <ul class="list-unstyled d-flex gap-4 ">
        <li v-for="( menu, i ) in menuEl">
            <a :class="index === i ? 'active' : ''" :href="menu.link" @click="selectMenuItem(i)">{{ menu.text }}</a>
            <svg xmlns="http://www.w3.org/2000/svg" width="10" height="10" fill="currentColor"
                class="bi bi-chevron-down" viewBox="0 0 16 16">
                <path fill-rule="evenodd"
                    d="M1.646 4.646a.5.5 0 0 1 .708 0L8 10.293l5.646-5.647a.5.5 0 0 1 .708.708l-6 6a.5.5 0 0 1-.708 0l-6-6a.5.5 0 0 1 0-.708z" />
            </svg>
        </li>
        <!--<li>
            <a href="#">Pages</a>
            <svg xmlns="http://www.w3.org/2000/svg" width="10" height="10" fill="currentColor"
                class="bi bi-chevron-down" viewBox="0 0 16 16">
                <path fill-rule="evenodd"
                    d="M1.646 4.646a.5.5 0 0 1 .708 0L8 10.293l5.646-5.647a.5.5 0 0 1 .708.708l-6 6a.5.5 0 0 1-.708 0l-6-6a.5.5 0 0 1 0-.708z" />
            </svg>
        </li>
        <li>
            <a href="#">Courses</a>
            <svg xmlns="http://www.w3.org/2000/svg" width="10" height="10" fill="currentColor"
                class="bi bi-chevron-down" viewBox="0 0 16 16">
                <path fill-rule="evenodd"
                    d="M1.646 4.646a.5.5 0 0 1 .708 0L8 10.293l5.646-5.647a.5.5 0 0 1 .708.708l-6 6a.5.5 0 0 1-.708 0l-6-6a.5.5 0 0 1 0-.708z" />
            </svg>
        </li>
        <li>
            <a href="#">Features</a>
            <svg xmlns="http://www.w3.org/2000/svg" width="10" height="10" fill="currentColor"
                class="bi bi-chevron-down" viewBox="0 0 16 16">
                <path fill-rule="evenodd"
                    d="M1.646 4.646a.5.5 0 0 1 .708 0L8 10.293l5.646-5.647a.5.5 0 0 1 .708.708l-6 6a.5.5 0 0 1-.708 0l-6-6a.5.5 0 0 1 0-.708z" />
            </svg>
        </li>
        <li>
            <a href="#">Blog</a>
            <svg xmlns="http://www.w3.org/2000/svg" width="10" height="10" fill="currentColor"
                class="bi bi-chevron-down" viewBox="0 0 16 16">
                <path fill-rule="evenodd"
                    d="M1.646 4.646a.5.5 0 0 1 .708 0L8 10.293l5.646-5.647a.5.5 0 0 1 .708.708l-6 6a.5.5 0 0 1-.708 0l-6-6a.5.5 0 0 1 0-.708z" />
            </svg>
        </li>
        <li>
            <a href="#">Shop</a>
            <svg xmlns="http://www.w3.org/2000/svg" width="10" height="10" fill="currentColor"
                class="bi bi-chevron-down" viewBox="0 0 16 16">
                <path fill-rule="evenodd"
                    d="M1.646 4.646a.5.5 0 0 1 .708 0L8 10.293l5.646-5.647a.5.5 0 0 1 .708.708l-6 6a.5.5 0 0 1-.708 0l-6-6a.5.5 0 0 1 0-.708z" />
            </svg>
        </li>-->
    </ul>
</template>
<style lang="scss" scoped>
@use '../assets/scss/variables' as *;

ul {
    margin-bottom: -1rem;

    li {
        a {
            text-decoration: none;
            margin-right: 0.25rem;
            font-size: 14px;
            font-weight: 600;
            color: $md-darker;
        }

        svg {
            cursor: pointer;
            margin-right: 0.25rem;
            color: $md-darker;
        }
    }

    .active {
        color: gray;
    }
}
</style>