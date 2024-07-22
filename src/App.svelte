<script>
	import WhoToFollow from "./components/WhoToFollow.svelte"
  import Trends from "./components/Trends.svelte"
  import Icon from "./components/Icon.svelte"
	import { users, trends, icons } from "./lib/info"

</script>

<div class="container">
  <img class="logo" src="src/assets/svg/premium.svg" alt="logo">

  <div class="grid-container">
    <main class="main">
      <Icon icons={icons.icon_home}/>
      <Icon icons={icons.icon_explore}/>
      <Icon icons={icons.icon_notifications}/>
      <Icon icons={icons.icon_messages}/>
      <Icon icons={icons.icon_lists}/>
      <Icon icons={icons.icon_bookmarks}/>
      <Icon icons={icons.icon_communities}/>
      <Icon icons={icons.icon_premium}/>
      <Icon icons={icons.icon_profile}/>
      <Icon icons={icons.icon_more}/>
      <button class="icon-button">
        Post
      </button>
    </main>
    
    <div class="spacer">
      <h1>Main Content</h1>
    </div>
    
    <aside class="aside">
      <h2>Who to follow</h2>
      <ul>
        <WhoToFollow user={users.user1}/>
        <WhoToFollow user={users.user2}/>
        <WhoToFollow user={users.user3}/>
      </ul>
      <a href="/" class="link">Show more</a>
      <h2 class="trends-header">Somplace trends</h2>
      <ul>
        <Trends trends={trends.trend1}/>
        <Trends trends={trends.trend2}/>
        <Trends trends={trends.trend3}/>
        <Trends trends={trends.trend4}/>
        <Trends trends={trends.trend5}/>
        <Trends trends={trends.trend6}/>
        <Trends trends={trends.trend7}/>
        <Trends trends={trends.trend8}/>
        <Trends trends={trends.trend9}/>
        <Trends trends={trends.trend10}/>
      </ul>
      <a href="/" class="link">Show more</a>
    </aside>
  </div>
</div>

<style>
.container {
    padding-left: 3rem;
    padding-right: 3rem;
}

.logo {
    padding-top: 1.5rem;
    padding-bottom: 1.5rem;
}

.grid-container {
    width: 100%;
    display: grid;
    grid-template-columns: 1fr 2fr 1fr; /* Ajuste para tener más espacio en la columna principal */
}

.main {
    grid-column: 1; /* Columna principal a la izquierda */
}

.spacer {
    grid-column: 2; /* Espacio vacío en el centro */
    padding-left: 0.5rem;
    padding-right: 0.5rem;
    font-size: 2.5rem;
    color: white;
}

.aside {
    grid-column: 3; /* Columna de aside a la derecha */
    padding-left: 0.5rem; /* px-2 */
    padding-right: 0.5rem;
    padding-bottom: 2.5rem; /* pb-10 */
}

.aside h2 {
    font-size: 1.875rem; /* text-3xl */
    font-weight: bold; /* font-bold */
}

.aside .trends-header {
    padding-top: 2.5rem; /* pt-10 */
    padding-bottom: 1.25rem; /* pb-5 */
}

.link {
    color: #3b82f6; /* text-blue-500 */
}

.icon-button {
    display: flex;
    align-items: center; /* items-center */
    margin-left: 1.25rem; /* ml-5 */
    margin-top: 0.75rem; /* mt-3 */
    padding-top: 0.5rem; /* py-2 */
    padding-bottom: 0.5rem;
    padding-left: 5rem; /* px-20 */
    padding-right: 5rem;
    font-size: 1.25rem; /* text-xl */
    border-radius: 9999px; /* rounded-full */
    background-color: #3b82f6; /* bg-blue-500 */
    color: white; /* text-white */
}

</style>