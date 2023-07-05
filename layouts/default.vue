<template>
    <div>
        <header class="shadow-sm bg-white p-4">
        <ul class="flex gap-4">
            <li><a href="/">Home</a></li>
            <li><a href="/about">Speakers</a></li>
        <li><a href="/products">Agenda</a></li>
        </ul>
    </header>
        <div class="container mx-auto p-4">
            <!--output the page content-->
        <slot />
        </div>

        <footer class="container mx-auto p-4 flex justify-between border-t-2">
            <ul class="flex gap-4">
                <li><a href="/">Home</a></li>
            <li><a href="/about">About</a></li>
            </ul>
        </footer>

    </div>

</template>