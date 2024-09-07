<script>

  import * as Card from "$lib/components/ui/card";
  import { Button } from "$lib/components/ui/button";
  import * as Avatar from "$lib/components/ui/avatar";
</script>

<main class="flex flex-col items-center p-4 space-y-6">
  <!-- Hero Section -->
  <section class="w-full bg-gray-800 text-white p-8 rounded-lg text-center">
    <h1 class="text-4xl font-bold">Welcome to My Technical Profile</h1>
    <p class="mt-4 text-lg">Exploring the world of technology and innovation</p>
  </section>

  <!-- Profile Section -->
  <Card.Root class="w-full max-w-md">
    <Card.Header class="flex flex-col items-center">
      <Avatar.Root class="w-24 h-24 mb-4">
        <Avatar.Image src="https://images.unsplash.com/photo-1603415526960-f8f0a5f0f6b1?w=800&dpr=2&q=80" alt="Profile Picture" class="rounded-full" />
        <Avatar.Fallback>JD</Avatar.Fallback>
      </Avatar.Root>
      <Card.Title class="text-2xl font-semibold">John Doe</Card.Title>
      <Card.Description class="text-center mt-2">
        A passionate developer with a love for creating innovative solutions.
      </Card.Description>
    </Card.Header>
    <Card.Content class="flex justify-center space-x-4 mt-4">
      <Button variant="outline">Follow</Button>
      <Button variant="outline">Message</Button>
    </Card.Content>
  </Card.Root>
</main>