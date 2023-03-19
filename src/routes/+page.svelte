<script>
    import Footer from "./footer.svelte";
import Header from "./header.svelte";
</script>

<style>
    @keyframes hero-text-slide-up-fade {
        0% {
            opacity: 0;
            transform: translateY(16px)
        }

        to {
            opacity: 1;
            transform: translateY(0)
        }
    }

    .animate-hero-text-slide-up-fade {
        animation: hero-text-slide-up-fade 1.2s ease-in-out; 
    }

    .animate-hero-text-slide-up-fade-delayed-200{
        animation: hero-text-slide-up-fade 1.2s ease-in-out 0.2s; 
        animation-fill-mode: forwards;
    }

    .animate-hero-text-slide-up-fade-delayed-400{
        animation: hero-text-slide-up-fade 1.2s ease-in-out 0.5s; 
        animation-fill-mode: forwards;
    }
</style>

<div class="w-full h-screen p-4">
    <Header/>
    <div class="h-[30vh]" />
    <div
        class="text-purple-400 font-medium max-w-fit px-2 py-0.5 bg-purple-900 rounded-sm bg-opacity-50 text-sm animate-hero-text-slide-up-fade"
    >
        Currently in private beta
    </div>
    <div
        class="text-3xl font-extrabold text-transparent bg-clip-text bg-gradient-to-r from-white to-slate-400 mt-3 animate-hero-text-slide-up-fade delay-700"
    >
        The new insight API for development teams
    </div>
    <div class="text-lg text-gray-500 mt-4 animate-hero-text-slide-up-fade-delayed-200 opacity-0">
        Say goodbye to the politics, competition, and inefficiencies that plague traditional work environments.
    </div>
    <button class="text-sm h-10 pl-4 pr-4 rounded-md gap-1 font-semibold bg-white text-black hover:bg-white/90 focus:ring-2 focus:ring-white/20 focus:outline-none focus:bg-white/90 items-center border justify-center select-none disabled:cursor-not-allowed disabled:opacity-70 transition ease-in-out duration-200 cursor-pointer inline-flex animate-hero-text-slide-up-fade-delayed-400 mt-6 opacity-0" style="box-shadow:-8px 0px 20px rgba(5, 162, 194, 0.3), 0px 0px 20px rgba(112, 225, 200, 0.3), 8px 0px 20px rgba(255, 178, 36, 0.3)">Request access</button>
    <Footer/>
</div>
