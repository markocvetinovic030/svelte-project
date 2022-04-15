<div class="bg-gray-50">

    <div class="container w-8/12 m-auto flex pt-20 pb-20">
        <div class=" w-1/2 p-10 text-center">
            <h1 class="font-bold text-5xl text-orange-500 pb-12">Welcome!</h1>
            <p class="p-10 text-orange-400 text-2xl font-bold">Lorem ipsum dolor sit amet, consectetur adipiscing elit.
                Fusce
                quis neque velit.</p>
            <p class="text-orange-400 text-xl mb-10">Lorem ipsum dolor sit amet.</p>

            <button id="signup" class="text-white font-bold bg-orange-400 p-2 mt-4 w-40 rounded-3xl  hover:bg-orange-600 transition-all duration-300">Signup</button>
        </div>

        <div class=" w-1/2 p-10">
            <form action="login" on:submit="{handleSubmit}">
                <form class="text-center">
                    <p class=" pb-12 text-orange-500 text-4xl font-bold">Login</p>
                    <label class=" text-orange-400 font-bold text-lg" for="fname">Username:</label><br>
                    <input
                        class="bg-orange-200 mt-4 mb-10 w-72 h-8 hover:bg-orange-300 transition-all duration-300 text-white p-6 outline-none rounded-3xl"
                        type="text" id="username" name="username"><br>
                    <label class=" text-orange-400 font-bold text-lg" for="password">Password:</label><br>
                    <input
                        class="bg-orange-200 mt-4 mb-10 w-72 h-8 hover:bg-orange-300 transition-all duration-300 text-white p-6 outline-none rounded-3xl"
                        type="password" id="password" name="password"><br>

                        <input class="text-white font-bold bg-orange-400 p-2 mt-4 w-40 rounded-3xl hover:bg-orange-600 transition-all duration-300" type="submit" id="submit" name="submit" >
                </form>
            </form>
        </div>
    </div>
</div>

<script>
    function handleSubmit() {
        console.log('Submited');
    }
</script>