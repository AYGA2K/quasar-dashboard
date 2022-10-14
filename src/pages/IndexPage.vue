<template>
  <q-page class="q-mx-md">
    <div class="row justify-between">
      <div>
        <div
          class="text-white text-h5 text-weight-bold"
        >
          Hello,Itachi
        </div>
        <div
          class="text-white text-subtitles-1 text-weight-bold"
        >
          Welcome Back!
        </div>
      </div>
      <div>
        <q-btn
          outline
          class="border-radius-10px"
          text-color="grey"
          align="left"
        >
          <div class="q-mr-xl q-my-sm">
            Filter
          </div>
          <q-icon name="tune" color="white" />
        </q-btn>
      </div>
    </div>
    <div class="row q-mt-sm justify-between">
      <q-card
        style="width: 30%"
        class="border-radius-10px bg-linear-secondary-primary"
      >
        <q-card-section>
          <div class="row justify-between">
            <q-icon
              class="border-radius-square-1"
              style="color: #0b1e51"
              size="md"
              name="trending_up"
            />

            <q-icon
              class="border-radius-circle"
              color="white"
              size="md"
              name="arrow_forward"
            />
          </div>
          <div class="q-mt-sm">
            <div
              class="text-white text-subtitle1 text-weight-bold"
            >
              $4522464
            </div>
            <div class="row justify-between">
              <div
                class="text-weight-bold"
                style="color: #667cb1"
              >
                Total Sales
              </div>
              <div
                class="text-white text-weight-bold q-ml-lg"
              >
                +32.40
              </div>
            </div>
          </div>
        </q-card-section>
      </q-card>
      <q-card
        style="width: 30%"
        class="border-radius-10px bg-linear-secondary-primary"
      >
        <q-card-section>
          <div class="row justify-between">
            <q-icon
              class="border-radius-square-2"
              style="color: #0b1e51"
              size="md"
              name="trending_up"
            />

            <q-icon
              class="border-radius-circle"
              color="white"
              size="md"
              name="arrow_forward"
            />
          </div>
          <div class="q-mt-sm">
            <div
              class="text-white text-subtitle1 text-weight-bold"
            >
              $4522464
            </div>
            <div class="row justify-between">
              <div
                class="text-weight-bold"
                style="color: #667cb1"
              >
                Total Sales
              </div>
              <div
                class="text-white text-weight-bold q-ml-lg"
              >
                +32.40
              </div>
            </div>
          </div>
        </q-card-section>
      </q-card>
      <q-card
        style="width: 30%"
        class="border-radius-10px bg-linear-secondary-primary"
      >
        <q-card-section>
          <div class="row justify-between">
            <q-icon
              class="border-radius-square-3"
              style="color: #0b1e51"
              size="md"
              name="trending_up"
            />

            <q-icon
              class="border-radius-circle"
              color="white"
              size="md"
              name="arrow_forward"
            />
          </div>
          <div class="q-mt-sm">
            <div
              class="text-white text-subtitle1 text-weight-bold"
            >
              $4522464
            </div>
            <div class="row justify-between">
              <div
                class="text-weight-bold"
                style="color: #667cb1"
              >
                Total Sales
              </div>
              <div
                class="text-white text-weight-bold q-ml-lg"
              >
                +32.40
              </div>
            </div>
          </div>
        </q-card-section>
      </q-card>
    </div>
    <div class="q-mt-sm">
      <ApexChart></ApexChart>
    </div>
    <div
      class="bg-linear-secondary-primary border-radius-10px q-pa-md"
    >
      <h2
        class="text-white text-h6 border-radius-10px"
      >
        Recent Transactions
      </h2>
      <div class="row justify-between">
        <h3
          class="text-subtitle2 text-weight-bold"
        >
          Company Name
        </h3>
        <h3
          class="text-subtitle2 q-ml-md text-weight-bold"
        >
          Date
        </h3>
        <h3
          class="text-subtitle2 text-weight-bold"
        >
          Amount
        </h3>
      </div>
      <div
        class="row justify-between items-center"
      >
        <div class="row q-mt-sm gap-1rem">
          <q-icon
            size="sm"
            class="border-radius-square-1 q-pa-sm"
            name="print"
          />
          <div>
            <h3
              class="text-white text-subtitle1 text-weight-bold"
            >
              Sikago and Sons
            </h3>
            <h4
              class="text-subtitle2 text-weight-bold"
            >
              15K
            </h4>
          </div>
        </div>
        <h3
          class="text-subtitle2 text-weight-bold"
        >
          10 Jan 2022
        </h3>
        <h3
          class="text-subtitle2 text-white text-weight-bold"
        >
          $207.45
        </h3>
      </div>
      <div
        class="row justify-between items-center"
      >
        <div class="row q-mt-sm gap-1rem">
          <q-icon
            size="sm"
            class="border-radius-square-2 q-pa-sm"
            name="print"
          />
          <div>
            <h3
              class="text-white text-subtitle1 text-weight-bold"
            >
              Sikago and Sons
            </h3>
            <h4
              class="text-subtitle2 text-weight-bold"
            >
              15K
            </h4>
          </div>
        </div>
        <h3
          class="text-subtitle2 text-weight-bold"
        >
          10 Jan 2022
        </h3>
        <h3
          class="text-subtitle2 text-white text-weight-bold"
        >
          $207.45
        </h3>
      </div>
      <div
        class="row justify-between items-center"
      >
        <div class="row q-mt-sm gap-1rem">
          <q-icon
            size="sm"
            class="border-radius-square-3 q-pa-sm"
            name="print"
          />
          <div>
            <h3
              class="text-white text-subtitle1 text-weight-bold"
            >
              Sikago and Sons
            </h3>
            <h4
              class="text-subtitle2 text-weight-bold"
            >
              15K
            </h4>
          </div>
        </div>
        <h3
          class="text-subtitle2 text-weight-bold"
        >
          10 Jan 2022
        </h3>
        <h3
          class="text-subtitle2 text-white text-weight-bold"
        >
          $207.45
        </h3>
      </div>
    </div>
  </q-page>
</template>

<script lang="ts">
import {
  defineAsyncComponent,
  defineComponent,
} from 'vue';
const ApexChart = defineAsyncComponent(
  () =>
    import(
      'src/components/charts/Examplechart2.vue'
    )
);

export default defineComponent({
  components: {
    ApexChart,
  },
});
</script>
<style lang="scss">
* {
  margin: 0%;
  padding: 0%;
}
.text-subtitle2 {
  color: $mini-title;
}
.border-radius-10px {
  border-radius: 20px !important;
  border: 2px;
}
.border-radius-circle {
  border-radius: 50% !important;

  background: rgb(11, 30, 81);
  background: linear-gradient(
    144deg,
    rgba(11, 30, 81, 1) 60%,
    rgba(21, 46, 95, 1) 100%
  );
}
.border-radius-square-1 {
  border-radius: 20% !important;

  background: rgb(199, 228, 12);
}
.border-radius-square-2 {
  border-radius: 20% !important;

  background: rgb(43, 208, 230);
}
.border-radius-square-3 {
  border-radius: 20% !important;

  background: rgb(130, 22, 203);
}
.bg-linear-secondary-primary {
  background: linear-gradient(
    144deg,
    rgba(21, 46, 95, 1) 20%,
    $primary
  );
}
.gap-1rem {
  gap: 1rem;
}
</style>
