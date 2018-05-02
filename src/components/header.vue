<template>
    <header>
        <nav>
            <ul>
                <li><a href="">博客</a></li>
                <li><a href="">关于</a></li>
                <li><a href="">有趣的东西</a></li>
            </ul>
        </nav>
        <aside>
            <ul>
                <li><a href="">注册</a></li>
                <li><a href="">登陆</a></li>
            </ul>
        </aside>
    </header>
</template>

<script>
</script>

<style scoped>
* {
    margin: 0;
}

header {
    position: absolute;
    top: 0;
    left: 0;
    z-index: 10;
    display: flex;
    justify-content: space-between;
    width: 100%;
    margin: 0, auto;
    background: #333;
    text-align: center;
}

ul {
    list-style-type: none;
    padding: 0px;
    display: flex;
}

nav {
    justify-content: flex-start;
}

aside {
    justify-content: flex-end;
}

a {
    text-decoration: none;
    text-align: center;
    color: #fff;
    display: block;
    padding: 10px;
}

a:hover {
    background-color: #555;
}
</style>
