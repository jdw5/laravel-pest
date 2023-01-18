<template>
    <div class="min-h-screen bg-inherit">
        <nav>
        </nav>

        <main>
            <div class="max-w-4xl mx-auto px-6 grid grid-cols-8 gap-12 mt-16">
                <aside class="col-span-2 border-r border-slate-200 space-y-6">
                    <ul>
                        <li>
                            <span href="#" class="font-bold text-lg text-slate-600 hover:text-slate-800 block py-1 transition duration-150 ease-in-out">
                                Name
                            </span>
                        </li>
                        <li>
                            <a href="#" class="font-bold text-lg text-slate-600 hover:text-slate-800 block py-1 transition duration-150 ease-in-out">
                                Feed
                            </a>
                        </li>
                    </ul>
                    <ul>
                        <li>
                            <a href="#" class="font-bold text-lg text-slate-600 hover:text-slate-800 block py-1 transition duration-150 ease-in-out">
                                My Books
                            </a>
                        </li>
                    </ul>
                    <ul>
                        <li>
                            <a href="#" class="font-bold text-lg text-slate-600 hover:text-slate-800 block py-1 transition duration-150 ease-in-out">
                                Logout
                            </a>
                        </li>
                    </ul>
                </aside>
                <div class="col-span-6">
                    <h1 class="font-bold text-2xl text-slate-800">
                        <slot name="header" />
                    </h1>

                <slot />
                </div>
            </div>
        </main>
    </div>
</template>

<script>
    export default {
        props: {
            headeer: String
        }
    }
</script>
