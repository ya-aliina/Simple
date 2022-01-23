<template>
    <div data-vue-component="Content">
        <div class="container width">
            <div class="row">
                <div class="col-8">
                    <div class="title">
                        Настройки профиля
                    </div>
                </div>
            </div>
            <div class="row">
                <div class="col-12">
                    <form>
                        <div class="form-row">
                            <div class="col">
                                <input type="text" class="form-control" placeholder="Имя">
                            </div>
                            <div class="col">
                                <input type="text" class="form-control" placeholder="Фамилия">
                            </div>
                        </div>
                        <div class="row pt-3">
                            <div class="col">
                                <input class="form-control" type="text" placeholder="Отчество">
                            </div>
                        </div>
                        <div class="form-group">
                            <label for="exampleInputEmail1">Email адрес</label>
                            <input type="email" class="form-control" id="exampleInputEmail1" aria-describedby="emailHelp" placeholder="Введите email">
                        </div>
                        <div class="form-group">
                            <label for="exampleInputPassword1">Пароль</label>
                            <input type="password" class="form-control" id="exampleInputPassword1" placeholder="Пароль">
                            <small id="passwordRools" class="form-text text-muted">Ваш пароль должен состоять из 8-20 символов, содержать буквы и цифры и не должен содержать пробелов, специальных символов или эмодзи.</small>
                        </div>
                        <button type="submit" class="btn btn-primary">Сохранить изменения</button>
                    </form>
                </div>
            </div>
        </div>

    </div>
</template>

<script>

export default {
    name: "Content",
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

.title {
    font: 16px Roboto;
    font-weight: 500;
    flex-grow: 1;
    margin: 0 0 12px;
    letter-spacing: .1em;
    text-transform: uppercase;
    color: #8d98a2;
    padding: 30px 0;
}
.width {
    width: 100vw;
    margin: 0 auto;
}

</style>