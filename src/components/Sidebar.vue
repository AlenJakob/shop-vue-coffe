<template>
  <section>
    <b-sidebar
      type="is-light"
      :fullheight="fullheight"
      :fullwidth="fullwidth"
      :right="right"
      v-model="open"
    >
      <div class="p-3">
        <img
          src="../assets/logo.png"
          alt="Lightweight UI components for Vue.js based on Bulma"
        />
        <b-menu>
          <b-menu-list>
            <!--  -->
            <b-menu-item>
              <template slot="label">Home</template>
            </b-menu-item>

            <b-menu-item>
              <template slot="label" slot-scope="props">
                Shop
                <b-icon
                  class="is-pulled-right"
                  :icon="props.expanded ? 'minus' : 'plus'"
                ></b-icon>
              </template>
              <b-menu-item label="Product Category"></b-menu-item>
              <b-menu-item label="Top rated product"> </b-menu-item>
            </b-menu-item>
            <!--  -->
            <b-menu-item>
              <template slot="label" slot-scope="props">
                Blog
                <b-icon
                  class="is-pulled-right"
                  :icon="props.expanded ? 'minus' : 'plus'"
                ></b-icon>
              </template>
              <b-menu-item label="Left Sidebar"></b-menu-item>
              <b-menu-item label="Right Sidebar"> </b-menu-item>
              <b-menu-item label="Full Width"> </b-menu-item>
            </b-menu-item>
            <!--  -->
            <b-menu-item>
              <template slot="label" slot-scope="props">
                Media
                <b-icon
                  class="is-pulled-right"
                  :icon="props.expanded ? 'minus' : 'plus'"
                ></b-icon>
              </template>
              <b-menu-item>
                <template slot="label" slot-scope="props">
                  Gallery
                  <b-icon
                    class="is-pulled-right"
                    :icon="props.expanded ? 'minus' : 'plus'"
                  ></b-icon>
                </template>
                <b-menu-item label="1 columns"> </b-menu-item>
                <b-menu-item label="2 columns"> </b-menu-item>
              </b-menu-item>
              <b-menu-item>
                <template slot="label" slot-scope="props">
                  Portfolio
                  <b-icon
                    class="is-pulled-right"
                    :icon="props.expanded ? 'minus' : 'plus'"
                  ></b-icon>
                </template>
                <b-menu-item label="3 columns"> </b-menu-item>
                <b-menu-item label="4 columns"> </b-menu-item>
              </b-menu-item>
            </b-menu-item>
            <!--  -->
          </b-menu-list>

          <b-menu-list label="Actions">
            <b-menu-item label="Logout"></b-menu-item>
          </b-menu-list>
        </b-menu>
      </div>
    </b-sidebar>
  </section>
</template>

    <script>
export default {
  data() {
    return {
      open: false,
      overlay: true,
      fullheight: true,
      fullwidth: false,
      right: false,
    };
  },
  mounted() {
    document
      .querySelector(".burger")
      .addEventListener("click", () => (this.open = !this.open));
  },
};
</script>