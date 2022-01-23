<template>
    <header>
        <nav>
            <div class="row">
                <div class="col-3 logo">
                    <a href="#"><img src="../assets/icons/logo.svg" alt="logo" class="logo_img"></a>
                </div>
                <div class="offset-1 col-3 pt-10">

                </div>
                <div class="offset-2 col-3 ">
                    <ul class="user_notification">
                        <li class="user_notification_item">
                            <a href="#"><img src="../assets/icons/message.svg" alt="message"></a>
                        </li>
                        <li class="user_notification_item">
                            <a href="#"><img src="../assets/icons/notification.svg" alt="notification"></a>
                        </li>
                        <li class="user_notification_item">
                            <a href="#"><img src="../assets/icons/profile.svg" alt="profile"></a>
                        </li>
                    </ul>
                </div>
            </div>
        </nav>
    </header>
</template>

<script>
export default {
    name: "Header",
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
header, nav {
    background: #FFFF;
    height: 64px;
    /*position: fixed;*/
    width: 100%;
    z-index: 20;
}

.row {
    max-height: 64px;
    box-shadow: 0 0 4px rgba(66,72,78,.12),0 1px 2px rgba(66,72,78,.08),0 0 1px rgba(66,72,78,.08);
}

.logo {
    display: flex;
    justify-content: end;
    padding-left: 0px;
}

.logo_img {
    display: flex;
    align-items: end;
    box-sizing: border-box;
    width: auto;
    height: auto;
    max-height: 64px;
}

.user_notification_item {
    display: flex;
    width: 35px;
    height: 35px;
    justify-content: center;
    align-items: center;
    background: rgba(66, 72, 78, 0.08);
    border-radius: 50%;
}

.user_notification_item:hover {
    background: rgba(66, 72, 78, 0.24);
}

.user_notification_item a img{
    box-sizing: border-box;
    width: 20px;
    height: 20px;
    justify-content: center;
}

.user_notification {
    display: flex;
    list-style: none;
    height: 64px;
    justify-content: space-between;
    align-items: center;
    padding-left: 0;
    max-width: 165px;
}

</style>