<template>

  <b-container >
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
          <b-col sm="12">
          <b-card class="mt-1 rounded shadow-sm" style="background-color: #1f2937" text-variant="light">
            <span class="text-light font-weight-bold">My tags</span> <br>
            <hr>
            <b-row>
              <b-col>
                <b-badge variant="dark">
                  Antonio Fabrizio Fiume
                </b-badge>
              </b-col>
              <b-col>
                <b-badge>
                  https://github.com/FabriGinseng
                </b-badge>
              </b-col>
              <b-col>
                <b-badge variant="danger ">
                  Italy
                </b-badge>
              </b-col>
              <b-col>
                <b-badge variant="primary">
                  Software developer
                </b-badge>
              </b-col>
              <b-col>
                <b-badge variant="success">
                  Mobile developer
                </b-badge>
              </b-col>
              <b-col>
                <b-badge variant="primary">
                  Xamarin developer
                </b-badge>
              </b-col>
              <b-col>
                <b-badge variant="dark">
                  C#
                </b-badge>
              </b-col>
              <b-col>
                <b-badge variant="success">
                  VueJS
                </b-badge>
              </b-col>
              <b-col>
                <b-badge variant="warning">
                  JavaScript
                </b-badge>
              </b-col>
              <b-col>
                <b-badge variant="dark">
                  Team Work
                </b-badge>
              </b-col>
              <b-col>
                <b-badge variant="primary">
                  engineering
                </b-badge>
              </b-col>
              <b-col>
                <b-badge variant="success">
                  frontend developer
                </b-badge>
              </b-col>
              <b-col>
                <b-badge variant="warning">
                  Improve yourself
                </b-badge>
              </b-col>
              <b-col>
                <b-badge variant="dark">
                  bachelor's degree in computer engineering
                </b-badge>
              </b-col>
            </b-row>
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
