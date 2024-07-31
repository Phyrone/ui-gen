<script>

  import { Button } from "$lib/components/ui/button";
  import { Card } from "$lib/components/ui/card";
</script>

<style>
  .background {
    background-image: url('https://images.unsplash.com/photo-1501594907352-04cda38ebc29?w=1600&dpr=2&q=80');
    background-size: cover;
    background-position: center;
    height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
  }
  .content {
    background: rgba(255, 255, 255, 0.8);
    border-radius: 1rem;
    padding: 2rem;
    text-align: center;
    max-width: 400px;
  }
  .title {
    font-size: 2rem;
    font-weight: bold;
    color: #ff69b4;
  }
  .description {
    font-size: 1rem;
    color: #ff69b4;
    margin-bottom: 1rem;
  }
</style>

<div class="background">
  <div class="content">
    <Card.Root>
      <Card.Header>
        <Card.Title class="title">Welcome to Cute World!</Card.Title>
      </Card.Header>
      <Card.Content>
        <p class="description">Everything here is cute and lovely. Enjoy your stay!</p>
      </Card.Content>
      <Card.Footer>
        <Button variant="outline">Get Started</Button>
      </Card.Footer>
    </Card.Root>
  </div>
</div>