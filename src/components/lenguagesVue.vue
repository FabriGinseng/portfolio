<template>
  <b-container>
    <b-card variant="dark" class="shadow-lg rounded mt-5">
      <span class="text-dark font-weight-bold">{{$t('messagePercentage')}} </span>
      <br />
      <span class="text-secondary"> {{$t('subtitlePercentage')}}</span>
      <hr />
      <br />
      <div v-for="bar in bars" :key="bar.value" class="row mb-2">
        <div class="col-md-7">
          <b-badge class="text-white col-ms-1" variant="dark">
            {{bar.title }}
          </b-badge>
          <b-progress
            :value="bar.value"
            :variant="bar.variant"
            striped
            animated="animated"
          ></b-progress>
        </div>
      </div>
      <br />
    </b-card>
  </b-container>
</template>
<script>
export default {
    name: 'lenguagesVue',
    data() {
        return {
            bars: [
              {title: "Xamarin", value: 80, variant: "primary"},
              {title: "Vue JS", value: 60, variant: "success"},
              {title: "C#", value: 80, variant: "primary"},
              {title: "Electron", value: 55, variant: "success"},
              {title: "Windows form", value: 35, variant: "warning"},
              {title: "NodeJs", value: 45, variant: "primary"},
              {title: "JavaScript", value:70, variant: "warning"},
              {title: "TypeScript", value: 40, variant: "primary"},
            ]
        }
    }
}
</script>
