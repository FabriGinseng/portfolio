<template>

    <b-container>
     <b-card class="mt-5 rounded shadow-lg" style="background-color: #1f2937" text-variant="light">
          <span class="text-light font-weight-bold">{{$t('messageProfileTitle')}}</span> <br>
          <hr>
          <p>
           {{$t('messageProfile')}}
            </p>

     </b-card>
    </b-container>


</template>

<script>
export default {
    name: 'profileVue'
}
</script>
