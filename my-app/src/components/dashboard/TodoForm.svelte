<script>
  export let todoInput;
  export let add;
</script>

      <div>
        
        <h2 class="mt-6 text-center text-3xl font-bold tracking-tight text-gray-900">Welcome to your to do list</h2>
       
      </div>
      <form class="mt-8 space-y-6" on:submit={add}>
        <input type="hidden" name="remember" value="true">
        <div class="-space-y-px rounded-md shadow-sm">
          <div>
            <label for="todo-input" class="sr-only">Email address</label>
            <input bind:value={todoInput} id="todo-input"  type="text"  required class="relative block w-full appearance-none rounded-none rounded-t-md border border-gray-300 px-3 py-2 text-gray-900 placeholder-gray-500 focus:z-10 focus:border-indigo-500 focus:outline-none focus:ring-indigo-500 sm:text-sm" placeholder="Enter a todo">
          </div>
          
        </div>
            
        <div>
          <button type="submit" class="group relative flex w-full justify-center rounded-md border border-transparent bg-indigo-600 py-2 px-4 text-sm font-medium text-white hover:bg-indigo-700 focus:outline-none focus:ring-2 focus:ring-indigo-500 focus:ring-offset-2">
            <span class="absolute inset-y-0 left-0 flex items-center pl-3">
              <!-- Heroicon name: mini/lock-closed -->
              
                
            </span>
            Add todo
          </button>
        </div>
      </form>
