<template>
  <div class="navbar">
    <div
      class="menu-icon"
      v-for="tab in tabs"
      :key="tab"
      @click="changeTab(tab)"
      :class="{ 'active': currentTab === tab }"
    ></div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      tabs: ['tab1', 'tab2', 'tab3'],
      currentTab: 'tab1',
    };
  },
  methods: {
    changeTab(tab) {
      this.currentTab = tab;
      this.$emit('tab-change', tab);
    },
    handleScroll(event) {
      if (event.deltaY > 0) {
        // Desplazamiento hacia abajo (scroll hacia arriba)
        const currentIndex = this.tabs.indexOf(this.currentTab);
        if (currentIndex < this.tabs.length - 1) {
          this.changeTab(this.tabs[currentIndex + 1]);
        }
      } else if (event.deltaY < 0) {
        // Desplazamiento hacia arriba (scroll hacia abajo)
        const currentIndex = this.tabs.indexOf(this.currentTab);
        if (currentIndex > 0) {
          this.changeTab(this.tabs[currentIndex - 1]);
        }
      }
    },
  },
  mounted() {
    window.addEventListener('wheel', this.handleScroll, { passive: true });
  },
  beforeDestroy() {
    window.removeEventListener('wheel', this.handleScroll);
  },
};
</script>

<style>
.navbar {
  display: flex;
  justify-content: center;
  align-items: center;
  background-color: #000;
  padding: 10px;
}

.menu-icon {
  width: 10px;
  height: 10px;
  background-color: #827d7d;
  border-radius: 50%;
  margin: 0 10px;
  cursor: pointer;
  transition: background-color 0.3s;
}

.menu-icon:focus {
  background-color: #fff;
}

.active {
  background-color: #fff;
}
</style>
