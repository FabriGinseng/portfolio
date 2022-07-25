<template>

  <b-container >
    <br>
          <span class="text-light font-weight-bold mt-2">Su di me</span>
    <br>
          <hr>
        <b-row>
          <b-col sm="12" >
            <b-card class="my-2 shadow-lg" style="background-color: #1f2937" text-variant="light">
              <span class="text-light;">Fabrizio</span>
              <hr>
              {{$t('messageAboutMe')}}

            </b-card>
          </b-col>
          <b-col sm="12">
            <b-card class="my-2 shadow-lg" style="background-color: #1f2937" text-variant="light">
              <span class="text-light" >{{$t('messageTitleExperience')}}</span>
              <hr>
             {{$t('messageExperience')}}
            </b-card>
          </b-col>
        </b-row>
      </b-container>

</template>

<script>
export default {
    name: 'aboutVue'
}
</script>
