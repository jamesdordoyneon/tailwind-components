<template>
    <div class="side-bar lg:w-1/6 sm:w-full">
        <div class="side-bar-header">
            <div class="side-bar-details flex flex-wrap">
                <div class="side-bar-img lg:w-1/4">
                    <img class="rounded-img" src="/img/me.jpeg">
                </div>
                <div class="side-bar-details lg:w-3/2">
                    <p class="text-white pb-2">James Dordoy</p>
                    <p><i class="fa fa-circle text-green" aria-hidden="true"></i>
                    <span class="text-white">Online</span> </p>
                </div>
            </div>

            <div class="side-bar-search">
                <input class="shadow appearance-none border rounded w-full py-2 px-3 text-grey-darker leading-tight" id="username" type="text" placeholder="Search">
            </div>
        </div>
        <div class="side-bar-navigation">
            <p class="block bg-black">Navigation</p>
            <hr>
        </div>
    </div>
</template>

<style scoped>

</style>

<script>

export default {

}

</script>