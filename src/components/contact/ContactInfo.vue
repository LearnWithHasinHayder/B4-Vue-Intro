<script setup>
defineProps(['phone', 'email', 'address'])
</script>

<template>
    <div class="lg:mb-0 mb-10">
        <div class="group w-full h-full">
            <div class="relative h-full">
                <img src="/images/contact.jpeg" alt="ContactUs tailwind section" class="w-full h-full lg:rounded-l-2xl rounded-2xl bg-blend-multiply" />
                <h1 class="font-manrope text-black text-4xl font-bold leading-10 absolute top-11 left-11">Contact us</h1>
                <div class="absolute bottom-0 w-full lg:p-11 p-5">
                    <div class="bg-white rounded-lg p-6 block">
                        <a href="#" class="flex items-center mb-6">
                            <i class="bi bi-telephone"></i>
                            <h5 class="underline text-black text-base font-normal leading-6 ml-5"> {{ phone }} </h5>
                        </a>
                        <a href="mailto:pro@lingare.com" class="flex items-center mb-6">
                            <i class="bi bi-envelope"></i>
                            <h5 class="underline text-black text-base font-normal leading-6 ml-5"> {{ email }}</h5>
                        </a>
                        <a href="#" class="flex items-center">
                            <i class="bi bi-geo-alt"></i>
                            <h5 class="underline text-black text-base font-normal leading-6 ml-5">{{ address }}</h5>
                        </a>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped></style>