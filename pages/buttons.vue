<template>
  <v-container>
    <div class="home">
    <h1>HomePage</h1>
      <v-btn class="pink white--text">click me</v-btn>
      <v-btn depressed color="pink">click me</v-btn>
      <v-btn text color="pink">click me</v-btn>

      <v-btn depressed class="pink white--text">
        <v-icon left>mdi-email</v-icon>
        <span>email me</span>
      </v-btn>

      <v-btn depressed small class="pink white--text">
        <v-icon left small>mdi-email</v-icon>
        <span>email me</span>
      </v-btn>

      <v-btn depressed large class="pink white--text">
        <span>email me</span>
        <v-icon right large>mdi-email</v-icon>
      </v-btn>

      <v-btn fab depressed small dark color="purple">
        <v-icon>mdi-heart</v-icon>
      </v-btn>

    </div>
  </v-container>
</template>

<script>
export default {
}
</script>
