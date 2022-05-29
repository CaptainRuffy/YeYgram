<template>
  <div class="sidebar-page">
    <section class="sidebar-layout">
      <b-sidebar
        position="static"
        :mobile="mobile"
        :expand-on-hover="expandOnHover"
        :reduce="reduce"
        :delay="expandWithDelay ? 500 : null"
        type="is-light"
        open
      >
        <div class="p-1">
          <div class="block">
            <img
              src="image-removebg-preview.png"
              alt="Lightweight UI components for Vue.js based on Bulma"
            />
          </div>
          <b-menu class="is-custom-mobile">
            <b-menu-list label="Меню">
              <b-menu-item
                icon="information-outline"
                label="Новости"
              ></b-menu-item>
              <b-menu-item active expanded icon="settings" label="Главная">
                <b-menu-item icon="account" label="Друзья"></b-menu-item>
                <b-menu-item
                  icon="cellphone-link"
                  label="Сообщения"
                ></b-menu-item>
              </b-menu-item>
              <b-menu-item icon="account" label="Мой аккаунт">
                <b-menu-item
                  icon="account-box"
                  label="Моя страница"
                ></b-menu-item>
                <b-menu-item icon="home-account" label="Сторис"></b-menu-item>
              </b-menu-item>
            </b-menu-list>
            <b-menu-list>
              <b-menu-item label="Настройки" icon="link"></b-menu-item>
            </b-menu-list>
            <b-menu-list label="Другое">
              <b-menu-item icon="logout" label="Выход"></b-menu-item>
            </b-menu-list>
          </b-menu>
        </div>
      </b-sidebar>

      <div class="p-1">
        <b-field>
          <b-switch v-model="reduce">Reduced</b-switch>
        </b-field>
        <b-field>
          <b-switch v-model="expandOnHover">Expand on hover</b-switch>
        </b-field>
        <b-field>
          <b-switch v-model="expandWithDelay">Hover with delay</b-switch>
        </b-field>
        <b-field label="Mobile Layout">
          <b-select v-model="mobile">
            <option :value="null"></option>
            <option value="reduce">Reduced</option>
            <option value="hide">Hidden</option>
            <option value="fullwidth">Fullwidth</option>
          </b-select>
        </b-field>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  data() {
    return {
      expandOnHover: false,
      expandWithDelay: false,
      mobile: "reduce",
      reduce: false,
    };
  },
};
</script>

margin-bottom: 0; } } } } } }
