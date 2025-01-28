<script setup lang="ts">
import { Head, Link } from '@inertiajs/vue3';

defineProps<{
    canLogin?: boolean;
    canRegister?: boolean;
}>();

</script>

<template>

    <Head title="Welcome" />
    <div class="h-screen">
        <div class="bg-gray-50 text-black/50 dark:bg-stone-800 dark:text-emerald-500">
            <div class="flex flex-1 justify-around py-6 px-6 items-center">
                <div class="text-6xl">Shop</div>
                <div class="text-2xl">Mens</div>
                <div class="text-2xl">Womens</div>
                <div class="text-2xl">Kids</div>
                <div class="flex items-center space-x-2">
                    <Link href="#" class="flex items-center space-x-1">
                    <span class="pr-2">Basket</span>
                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5"
                        stroke="currentColor" class="size-4">
                        <path stroke-linecap="round" stroke-linejoin="round"
                            d="M15.75 10.5V6a3.75 3.75 0 1 0-7.5 0v4.5m11.356-1.993 1.263 12c.07.665-.45 1.243-1.119 1.243H4.25a1.125 1.125 0 0 1-1.12-1.243l1.264-12A1.125 1.125 0 0 1 5.513 7.5h12.974c.576 0 1.059.435 1.119 1.007ZM8.625 10.5a.375.375 0 1 1-.75 0 .375.375 0 0 1 .75 0Zm7.5 0a.375.375 0 1 1-.75 0 .375.375 0 0 1 .75 0Z" />
                    </svg>
                    </Link>
                </div>
            </div>
        </div>
        <div class="flex justify-around pt-6 text-6xl">MENS</div>
        <div class="grid grid-cols-4 gap-4 p-6">
            <div class="min-h-80 flex flex-col justify-center bg-gray-200">
                <div class="w-full h-full bg-cover bg-center bg-no-repeat" style="background-image: url('https://picsum.photos/500/');"></div>
                <p>Words</p>
                <p>Words</p>
                <p>Words</p>
            </div>
            <div class="min-h-80 flex items-center justify-center bg-gray-200 p-4">1</div>
            <div class="min-h-80 flex items-center justify-center bg-gray-200 p-4">1</div>
            <div class="min-h-80 flex items-center justify-center bg-gray-200 p-4">1</div>
            <div class="min-h-80 flex items-center justify-center bg-gray-200 p-4">1</div>
        </div>

    </div>
</template>
