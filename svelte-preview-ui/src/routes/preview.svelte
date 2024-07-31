<script>

  import { Button } from "$lib/components/ui/button";
  import { Input } from "$lib/components/ui/input";
  import { Label } from "$lib/components/ui/label";
  import { Separator } from "$lib/components/ui/separator";
  import { Github } from 'lucide-svelte';
</script>

<main class="flex h-screen">
  <!-- Left side with large image -->
  <div class="w-2/3 bg-gray-200">
    <img src="https://images.unsplash.com/photo-1506748686214-e9df14d4d9d0?w=800&dpr=2&q=80" alt="Login Image" class="object-cover w-full h-full" />
  </div>

  <!-- Right side with login form -->
  <div class="w-1/3 flex flex-col justify-center items-center p-8 bg-white rounded-l-lg shadow-lg">
    <h1 class="text-3xl font-bold mb-4">Login</h1>
    <form class="w-full max-w-sm">
      <div class="mb-4">
        <Label for="email">Email</Label>
        <Input id="email" type="email" placeholder="Enter your email" class="w-full mt-2" />
      </div>
      <div class="mb-4">
        <Label for="password">Password</Label>
        <Input id="password" type="password" placeholder="Enter your password" class="w-full mt-2" />
      </div>
      <Button class="w-full mb-4">Login</Button>
      <Separator class="my-4" />
      <div class="flex justify-center space-x-4">
        <Button variant="outline" class="flex items-center space-x-2">
          <Github />
          <span>Github</span>
        </Button>
      </div>
    </form>
  </div>
</main>

<style>
  main {
    font-family: 'Arial', sans-serif;
  }
</style>