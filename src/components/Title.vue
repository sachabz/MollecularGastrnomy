<template>
    <div class="title titlebg">
        <transition appear @before-enter="beforeEnter" @enter="enter">
            <h1 class="font-weight-bold">{{ title }}.</h1>
        </transition>
    </div>
</template>

<script>
import gsap from 'gsap'
export default {
    name: 'Title',
    props: {

        title: String,
    },
    setup() {
        const beforeEnter = (el) => {
            console.log("before enter - set initial state")
            el.style.transform = 'translateY(-60px)'
            el.style.opacity = 0
        }
        const enter = (el) => {
            console.log("starting")
            gsap.to(el, { duration: 1, y: 0, opacity: 1, ease: "bounce.out" });
        }
        return { beforeEnter, enter }
    }
}

</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.title {
    margin-top: 5rem;
}

.titlebg {
    background-color: rgba(255, 255, 255, 0.397);
}
</style>
