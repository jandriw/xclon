<script>
    export let trends = {
    id: 1, 
    type: "theme", 
    trend: "#GenericTrend", 
    posts: 9999,
    };
</script>

<div class="trend-container">
    <div class="trend-info">
        <span>{trends.id}</span>
        <span> · </span>
        <span>{trends.type}</span>
    </div>
    <div class="trend-title">{trends.trend}</div>
    <div class="trend-posts">{trends.posts} posts</div>
</div>

<style>
    .trend-container {
        padding-bottom: 1.25rem; 
        cursor: pointer;
    }

    .trend-info {
        display: flex;
        flex-grow: 1;
        margin-right: 0.5rem;
    }

    .trend-info span {
        font-size: 0.875rem; 
    }

    .trend-title {
        font-size: 1.125rem;
        font-weight: bold; 
    }

    .trend-posts {
        font-size: 0.875rem;
    }

</style>