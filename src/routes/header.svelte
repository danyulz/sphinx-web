<div class="animate-header-slide-down-fade">
    <div class="flex flex-row justify-between items-center">
        <div
            class="items-center max-w-fit text-2xl font-medium text-transparent bg-clip-text bg-gradient-to-r from-white to-purple-400 animate-hero-text-slide-up-fade delay-700"
        >
            Sphinx
        </div>
        <div class="flex flex-row items-center">
            <a href="/blog">
                <span
                    class="text-md text-slate-600 font-medium transition duration-200 ease-in-out hover:text-slate-12"
                    >Blog
                </span>
            </a>
            <a href="/docs">
                <span
                    class="text-md text-slate-600 font-medium transition duration-200 ease-in-out hover:text-slate-12 ml-4"
                    >Docs
                </span>
        </div>
    </div>
</div>

<style>
    @keyframes header-slide-down-fade {
        0% {
            opacity: 0;
            transform: translateY(-16px);
        }

        to {
            opacity: 1;
            transform: translateY(0);
        }
    }

    .animate-header-slide-down-fade {
        animation: header-slide-down-fade 1s ease-in-out;
    }
</style>
