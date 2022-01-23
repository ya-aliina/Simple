<template>
    <div data-vue-component="MenuSidebar">
        <ul class="sidebar menu">
            <li class="menu_item active">
                <a href="#"><img src="../assets/icons/main.png" alt="" class="menu_item_img"></a>
            </li>
            <li class="menu_item">
                <a href="#"><img src="../assets/icons/add.png" class="menu_item_img" alt=""></a>
            </li>
            <li class="menu_item">
                <a href="#"><img src="../assets/icons/files.png" class="menu_item_img" alt=""></a>
            </li>
            <li class="menu_item">
                <a href="#"><img src="../assets/icons/calendar.png" class="menu_item_img" alt=""></a>
            </li>
        </ul>


    </div>
</template>

<script>

export default {
    name: "MenuSidebar",
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
    .sidebar {
        background: #f6f6f7;
        box-shadow: 0 0 0 1px rgba(66,72,78,.14);
        display: flex;
        flex-direction: column;
        width: 64px;
        /*position: fixed;*/
        height: 100vh;
        z-index: 10;
    }

    .sidebar, menu {
        padding-left: 0;
        margin-bottom: 0;

    }

    .menu_item {
        list-style: none;
        display: flex;
        width: 48px;
        height: 48px;
        justify-content: center;
        padding: 8px;
        margin: 8px;
        position: relative;
    }

    .active::before {
        position: absolute;
        width: 4px;
        border-radius: 0 4px 4px 0;
        background: green;
    }

    .menu_item:hover,
    .active {
        background: rgba(50,53,55,.06);
        border-radius: 6px;
        transition: all .15s ease;
    }

    .menu_item_img {
        width: 24px;
        height: 24px;
    }

</style>