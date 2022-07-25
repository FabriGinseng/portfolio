<template>
  <b-container>
    <b-card variant="dark" class="shadow-lg rounded mt-5" style="background-color: #1f2937" text-variant="light">
      <span class="text-light font-weight-bold">{{$t('messageLevel')}} </span>
      <br />
      <span class="text-secondary"> {{$t('subtitleLevel')}}</span>
      <hr />
      <br />
      <div v-for="bar in bars" :key="bar.value" class="row mb-2">
        <div class="col">
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
    name: 'lenguagesRatingVue',
    data() {
        return {
            bars: [
              {title: "C#", value: 85, variant: "success"},
              {title: "Xamarin", value: 80, variant: "success"},
              {title: "JavaScript", value:70, variant: "primary"},
              {title: "Vue JS", value: 65, variant: "primary"},
              {title: "Electron", value: 55, variant: "warning"},
              {title: "NodeJs", value: 45, variant: "warning"},
              {title: "Windows form", value: 40, variant: "danger"},
              {title: "TypeScript", value: 40, variant: "danger"},
            ]
        }
    }
}
</script>
