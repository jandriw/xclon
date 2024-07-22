<script>
    export let user = {
      name: 'Nombre de Usuario',
      username: 'username',
      avatar: "/images/defaultuser.webp",
    };
</script>
  
<div class="user-container">
    <img src={user.avatar} alt="Avatar" class="user-avatar">
    <div class="user-info">
        <p class="user-name">{user.name}</p>
        <p class="user-username">@{user.username}</p>
    </div>
    <button class="follow-button">
        Follow
    </button>
</div>

<style>

.user-container {
    display: flex;
    align-items: center;
    cursor: pointer;
}

.user-avatar {
    background-color: #6b7280;
    width: 3rem;
    height: 3rem; 
    border-radius: 9999px; 
    margin-right: 1.5rem; 
}

.user-info {
    flex: 1;
    padding-left: 1rem;
    padding-right: 1rem; 
}

.user-name {
    font-weight: bold; 
    font-size: 1.125rem; 
    transition: text-decoration 0.2s;
}

.user-name:hover {
    text-decoration: underline;
}

.user-username {
    color: #4b5563;
}

.follow-button {
    background-color: #3b82f6;
    color: white;
    padding-top: 0.5rem;
    padding-bottom: 0.5rem;
    padding-left: 1rem;
    padding-right: 1rem;
    border-radius: 9999px; 
}
</style>