<template>
  <q-layout view="lHr lpR fFf" class="bg-primary">
    <q-header class="row justify-center">
      <q-icon
        color="white"
        name="menu"
        class="q-ma-md cursor-pointer fixed-top-left lt-md"
        @click="drawerLeft = !drawerLeft"
        size="md"
      />
      <div
        class="q-mt-sm bg-linear-secondary-primary border-radius-40px"
      >
        <q-input
          rounded
          borderless
          v-model="text"
          input-class="text-left text-white q-pa-sm "
        >
          <template v-slot:append>
            <q-icon
              class="q-pa-sm"
              v-if="text === ''"
              name="search"
              color="positive"
            />
            <q-icon
              v-else
              name="clear"
              @click="text = ''"
              color="positive"
              class="cursor-pointer q-pa-sm"
            />
          </template>
        </q-input>
      </div>
    </q-header>

    <q-drawer
      side="left"
      v-model="drawerLeft"
      :mini="miniState"
      :width="200"
      class="bg-primary"
    >
      <div>
        <q-icon
          color="white"
          name="menu"
          class="q-ma-md cursor-pointer gt-md"
          @click="miniState = !miniState"
          size="md"
        />
      </div>

      <q-list class="list-text">
        <q-item clickable v-ripple>
          <q-item-section avatar>
            <q-icon name="inbox" />
          </q-item-section>

          <q-item-section> Inbox </q-item-section>
        </q-item>

        <q-item
          active
          clickable
          v-ripple
          active-class="my-active-class"
        >
          <q-item-section avatar>
            <q-icon name="star" />
          </q-item-section>

          <q-item-section> Star </q-item-section>
        </q-item>

        <q-item clickable v-ripple>
          <q-item-section avatar>
            <q-icon name="send" />
          </q-item-section>

          <q-item-section> Send </q-item-section>
        </q-item>

        <q-item clickable v-ripple>
          <q-item-section avatar>
            <q-icon name="drafts" />
          </q-item-section>

          <q-item-section>
            Drafts
          </q-item-section>
        </q-item>
      </q-list>
    </q-drawer>
    <q-drawer
      side="right"
      v-model="drawerRight"
      :width="350"
      class="bg-primary q-pt-lg"
    >
      <q-list
        class="bg-secondary q-ma-md q-pa-md border-radius-15px"
      >
        <div class="row justify-end items-center">
          <q-icon
            class="q-mx-sm"
            size="sm"
            color="white"
            name="notifications"
          />
          <q-avatar class="q-mx-md" size="md">
            <img
              src="https://cdn.quasar.dev/img/avatar.png"
            />
          </q-avatar>
        </div>
        <div class="q-mx-sm">
          <p class="text-white text-bold">
            Recent Orders
          </p>
          <div
            class="row list-text justify-between text-subtitle2"
          >
            <p>Orders</p>
            <p class="q-px-lg">Amount</p>
          </div>
          <div class="q-gutter-y-md">
            <div
              class="row list-text justify-between"
            >
              <q-avatar size="lg" square>
                <img
                  src="https://cdn.quasar.dev/img/avatar.png"
                />
              </q-avatar>
              <div>
                <div class="text-white">
                  Thrsea Web
                </div>
                <div class="text-1rem">
                  2 minutes ago
                </div>
              </div>
              <p
                class="text-white bg-primary q-px-lg q-py-sm border-radius-10px"
              >
                1000$
              </p>
            </div>
            <div
              class="row list-text justify-between"
            >
              <q-avatar size="lg" square>
                <img
                  src="https://cdn.quasar.dev/img/avatar.png"
                />
              </q-avatar>
              <div>
                <div class="text-white">
                  Thrsea Web
                </div>
                <div class="text-1rem">
                  2 minutes ago
                </div>
              </div>
              <p
                class="text-white bg-primary q-px-lg q-py-sm border-radius-10px"
              >
                1000$
              </p>
            </div>
            <div
              class="row list-text justify-between"
            >
              <q-avatar size="lg" square>
                <img
                  src="https://cdn.quasar.dev/img/avatar.png"
                />
              </q-avatar>
              <div>
                <div class="text-white">
                  Thrsea Web
                </div>
                <div class="text-1rem">
                  2 minutes ago
                </div>
              </div>
              <p
                class="text-white bg-primary q-px-lg q-py-sm border-radius-10px"
              >
                1000$
              </p>
            </div>
          </div>
        </div>
      </q-list>
      <div
        class="bg-secondary q-ma-md q-pa-md border-radius-15px"
      >
        <ApexChart></ApexChart>
      </div>
    </q-drawer>
    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script lang="ts">
import {
  defineAsyncComponent,
  defineComponent,
} from 'vue';

const ApexChart = defineAsyncComponent(
  () =>
    import(
      'src/components/charts/Examplechart.vue'
    )
);
export default defineComponent({
  components: {
    ApexChart,
  },
  data(): {
    miniState: boolean;
    text: string;
    drawerLeft: boolean;
    drawerRight: boolean;
  } {
    return {
      miniState: false,
      text: '',
      drawerLeft: true,
      drawerRight: true,
    };
  },
});
</script>

<style lang="scss">
.bg-linear-secondary-primary {
  background: linear-gradient(
    144deg,
    rgba(21, 46, 95, 1) 20%,
    $primary
  );
}
.border-radius-40px {
  border-radius: 40px;
  border: 2px;
}
.border-radius-15px {
  border-radius: 15px;
  border: 2px;
}
.border-radius-10px {
  border-radius: 10px;
  border: 2px;
}
.my-active-class {
  background: linear-gradient(
    90deg,
    rgba(146, 103, 255, 1) 10%,
    rgba(146, 103, 255, 0) 100%
  );
  color: white;
}
.list-text {
  color: $menuItem;
  font-weight: bold;
}
.text-1rem {
  font-size: x-small;
}
.scroll {
  overflow: hidden !important;
}
aside {
  position: fixed !important;
  overflow: hidden !important;
}
</style>
