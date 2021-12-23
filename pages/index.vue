<template lang="pug">
  container()
    v-row
      v-col(cols=7)
        v-card
          v-card-title Form
          v-divider
          v-card-text
            v-text-field(outlined dense :label="test" :messages="schema.properties.comment.description")
      v-col(cols=5)
        v-card
          v-card-title Vieweraaa
          v-card-text
            | Here is viewer
</template>

<script>
import schema from '@/assets/json/schema.json'

export default {
  name: 'IndexPage',
  data() {
    return {
      schema,
      test: "teetet",
      comment: "",
      universeId: null,
      tickRate: 60.0,
      maxConcurrentAssetTransfers: 6,
      usernameOverride: null,
      loginCredential: "",
      loginPassword: "",
      startWorlds:[],
      dataFolder: null,
      cacheFoler: null,
      logsFolder: null,
      allowedUrlHosts: [],
      autoSpawnItems: [],
    }
  }
}
</script>
