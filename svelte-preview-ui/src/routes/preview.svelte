<script>

  import { Button } from "$lib/components/ui/button";
  import { Card } from "$lib/components/ui/card";
  import { Avatar } from "$lib/components/ui/avatar";
  import { Badge } from "$lib/components/ui/badge";
  import { Separator } from "$lib/components/ui/separator";
  import { Input } from "$lib/components/ui/input";
  import { Textarea } from "$lib/components/ui/textarea";
  import { Home, User, Search, ArrowRight } from 'lucide-svelte';
</script>

<style>
  :global(body) {
    font-family: 'Courier New', Courier, monospace;
    background-color: #f4f1de;
    color: #3d405b;
  }
</style>

<main class="p-8">
  <header class="flex items-center justify-between mb-8">
    <h1 class="text-4xl font-bold">Retro Portfolio</h1>
    <nav class="flex space-x-4">
      <Button variant="outline"><Home class="mr-2" /> Home</Button>
      <Button variant="outline"><User class="mr-2" /> About</Button>
      <Button variant="outline"><Search class="mr-2" /> Search</Button>
    </nav>
  </header>

  <section class="mb-8">
    <Card>
      <Card.Header>
        <Card.Title>Whoami</Card.Title>
        <Card.Description>A brief introduction about myself</Card.Description>
      </Card.Header>
      <Card.Content>
        <div class="flex items-center space-x-4">
          <Avatar>
            <Avatar.Image src="https://images.unsplash.com/photo-1502767089025-6572583495b9?w=800&dpr=2&q=80" />
            <Avatar.Fallback>AB</Avatar.Fallback>
          </Avatar>
          <p>Hi, I'm Alex, a web developer with a passion for creating beautiful and functional websites. I love coding, coffee, and retro games.</p>
        </div>
      </Card.Content>
    </Card>
  </section>

  <Separator />

  <section class="mb-8">
    <Card>
      <Card.Header>
        <Card.Title>Projects</Card.Title>
        <Card.Description>Some of my recent works</Card.Description>
      </Card.Header>
      <Card.Content>
        <ul class="space-y-4">
          <li>
            <Card>
              <Card.Header>
                <Card.Title>Project One</Card.Title>
                <Card.Description>A cool project I worked on</Card.Description>
              </Card.Header>
              <Card.Content>
                <p>This project is a web application that helps users track their tasks and manage their time effectively.</p>
              </Card.Content>
            </Card>
          </li>
          <li>
            <Card>
              <Card.Header>
                <Card.Title>Project Two</Card.Title>
                <Card.Description>Another awesome project</Card.Description>
              </Card.Header>
              <Card.Content>
                <p>This project is a mobile app that allows users to find the best coffee shops in their area.</p>
              </Card.Content>
            </Card>
          </li>
        </ul>
      </Card.Content>
    </Card>
  </section>

  <Separator />

  <section class="mb-8">
    <Card>
      <Card.Header>
        <Card.Title>Social Media</Card.Title>
        <Card.Description>Connect with me on social media</Card.Description>
      </Card.Header>
      <Card.Content>
        <ul class="space-y-4">
          <li>
            <Button variant="outline"><ArrowRight class="mr-2" /> Twitter</Button>
          </li>
          <li>
            <Button variant="outline"><ArrowRight class="mr-2" /> LinkedIn</Button>
          </li>
          <li>
            <Button variant="outline"><ArrowRight class="mr-2" /> GitHub</Button>
          </li>
        </ul>
      </Card.Content>
    </Card>
  </section>

  <Separator />

  <section class="mb-8">
    <Card>
      <Card.Header>
        <Card.Title>Blog Overview</Card.Title>
        <Card.Description>Latest posts from my blog</Card.Description>
      </Card.Header>
      <Card.Content>
        <ul class="space-y-4">
          <li>
            <Card>
              <Card.Header>
                <Card.Title>Blog Post One</Card.Title>
                <Card.Description>Published on January 1, 2023</Card.Description>
              </Card.Header>
              <Card.Content>
                <p>This blog post discusses the latest trends in web development and how to stay ahead of the curve.</p>
              </Card.Content>
            </Card>
          </li>
          <li>
            <Card>
              <Card.Header>
                <Card.Title>Blog Post Two</Card.Title>
                <Card.Description>Published on February 15, 2023</Card.Description>
              </Card.Header>
              <Card.Content>
                <p>This blog post explores the benefits of using Svelte for building modern web applications.</p>
              </Card.Content>
            </Card>
          </li>
        </ul>
      </Card.Content>
    </Card>
  </section>
</main>