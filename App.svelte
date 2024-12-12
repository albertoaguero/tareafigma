<script>
  import Header from './components/header.svelte';
  import Profile from './components/profile.svelte';
  import Options from './components/options.svelte';
  import Footer from './components/footer.svelte';

  let user = {
    name: "Juan Pelotas",
    username: "@juanelpelotas175",
    avatar: "https://via.placeholder.com/100",
    options: [
      { name: "Inversión", icon: "💹" },
      { name: "Hazte premium", icon: "💎" },
      { name: "Problemas/FAQ", icon: "📚" },
      { name: "Favoritos", icon: "❤️" },
      { name: "Contactos", icon: "📇" },
    ],
  };
</script>

<main>
  <Header />
  <Profile {user} />
  <Options {user} />
  <Footer />
</main>

<style>
  main {
    font-family: Arial, sans-serif;
    color: #333;
    margin: 0;
    padding: 0;
    display: flex;
    flex-direction: column;
    height: 100vh;
  }
</style>
