<template>
<div class="container mx-auto py-10">
    <div class="my-12 text-white">
            <h1 class="text-5xl font-light mb-4">
                Dashboard
            </h1>
            <h1 class="text-xl font-light">Welcome back, James</h1>
        </div>
        <div class="flex flex-wrap">
            <div class="w-full lg:w-1/3 mb-4">
                <div class="card bg-white lg:mr-2">
                    <div class="card-body">
                        <h1 class="text-5xl text-grey-darkest font-light mb-2">
                             112.758
                        </h1>
                        <span class="text-grey-darker uppercase tracking-wide">Page views</span>
                    </div>
                </div>
            </div>
            <div class="w-full lg:w-1/3 mb-4">
                <div class="card bg-white lg:mx-2">
                    <div class="card-body">
                        <h1 class="text-5xl text-grey-darkest font-light mb-2">4.632</h1>
                        <span class="text-grey-darker uppercase tracking-wide">Users registered</span>
                    </div>
                </div>
            </div>
            <div class="w-full lg:w-1/3 mb-4">
                <div class="card lg:ml-2">
                    <div class="card-body">
                        <daterange-picker
                            double
                            start-date="06/10/2017"
                            end-date="06/10/2018"
                            start-place-holders="12/01/2017"
                            end-place-holders="04/01/2018"
                            @get-dates="getDates"/>
                    </div>
                </div>
            </div>
            <div class="w-full mb-4">
                <div class="card bg-white">
                    <div class="card-header">
                        Page views in the last days
                    </div>
                    <div class="flex flex-wrap justify-around p-6">
                        <div>
                            <div class="flex flex-no-wrap justify-between items-center">
                                <h1 class="text-5xl text-grey-darkest font-light mb-2">1.952</h1>
                                <span class="text-grey-dark">(25%)</span>
                            </div>
                            <span class="text-grey-darker uppercase tracking-wide">Page views this month</span>
                        </div>
                        <div>
                            <h1 class="text-5xl text-grey-darkest font-light mb-2">$12.286</h1>
                            <span class="text-grey-darker uppercase tracking-wide">Estimated income</span>
                        </div>
                    </div>
                </div>
            </div>
            <div class="w-full md:w-1/2 xl:w-1/4">
                <div class="card bg-white mr-2">
                    <div class="card-body">
                        <h1 class="text-5xl text-grey-darkest font-light">
                            8.21
                            <span class="text-grey-dark text-2xl">GB</span>
                        </h1>
                        <span class="text-grey-darker uppercase tracking-wide">Storage used</span>
                    </div>
                </div>
            </div>
            <div class="w-full md:w-1/2 xl:w-1/4">
                <div class="card bg-white md:ml-2 xl:mx-2">
                    <div class="card-body">
                        <h1 class="text-5xl text-grey-darkest font-light">
                            2.1
                            <span class="text-grey-dark text-2xl">GB</span>
                        </h1>
                        <span class="text-grey-darker uppercase tracking-wide">Ram usage</span>
                    </div>
                </div>
            </div>
            <div class="w-full md:w-1/2 xl:w-1/4">
                <div class="card bg-white md:mr-2 xl:mx-2">
                    <div class="card-body">
                        <h1 class="text-5xl text-grey-darkest font-light">
                            88
                            <span class="text-grey-dark text-2xl">%</span>
                        </h1>
                        <span class="text-grey-darker uppercase tracking-wide">CPU load</span>
                    </div>
                </div>
            </div>
            <div class="w-full md:w-1/2 xl:w-1/4">
                <div class="card bg-white ml-2">
                    <div class="card-body">
                        <h1 class="text-5xl text-grey-darkest font-light">
                            720
                            <span class="text-grey-dark text-2xl">GB</span>
                        </h1>
                        <span class="text-grey-darker uppercase tracking-wide">Bandwidth used</span>
                    </div>
                </div>
            </div>
        </div>


</div>

</template>

<script>

    export default {
        props: {

        },
        mounted: function () {

        },
        methods: {
            getDates(e) {
                console.log("Start Date: " + e.startDate);
                console.log("End Date: " + e.endDate);
            }
        }
    }
</script>
