<script>
    export let icons = {
    icon: "/svg/favicon.png", 
    name: "theme",
    };
</script>

<button class="button">
    <img src={icons.icon} alt={icons.name} />
    <p class="icon-name">{icons.name}</p>
</button>

<style>
    .button {
        display: flex;
        align-items: center;
        padding-top: 0.1rem;
        padding-bottom: 0.1rem;
        margin-bottom: 10px;
        padding-left: 1rem;
        padding-right: 1rem;
        border-radius: 9999px;
        transition: background-color 0.2s;
    }

    .button:hover {
        background-color: #3b82f6;
    }

    .icon-name {
        padding-left: 0.75rem;
        font-size: 1rem;
        font-weight: 700;
    }

</style>