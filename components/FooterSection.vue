<!-- components/Footer.vue -->
<template>
    <footer class="footer">
        <div>
            <a href="https://github.com/yourusername" target="_blank" aria-label="GitHub">
                <font-awesome-icon :icon="['fab', 'github']" />
            </a>
            <a href="https://instagram.com/yourusername" target="_blank" aria-label="Instagram">
                <font-awesome-icon :icon="['fab', 'instagram']" />
            </a>
            <a href="https://facebook.com/yourusername" target="_blank" aria-label="Facebook">
                <font-awesome-icon :icon="['fab', 'facebook']" />
            </a>
            <a href="mailto:your-email@gmail.com" target="_blank" aria-label="Gmail">
                <font-awesome-icon :icon="['fas', 'envelope']" />
            </a>
        </div>
        <p>&copy; 2024 RasyifIbnuCorporate. All rights reserved.</p>
    </footer>
</template>

<script>
export default {
    name: 'Footer'
}
</script>

<style scoped>
.footer {
    background-color: #2c3e50;
    color: white;
    padding: 20px 0;
    text-align: center;
}
.footer a {
    color: white;
    margin: 0 15px;
    font-size: 20px;
    transition: color 0.3s;
}
.footer a:hover {
    color: #18bc9c;
}
.footer p {
    margin: 10px 0 0;
}
</style>
