<template>
  <v-container fluid class="blue-grey lighten-5 pa-0">
    <v-col class="mt-4" :class="dynamicPosition" cols="12" md="3" lg="3" xl="2">
      <v-row>
        <v-col>
          <ProfileSummary :key="3" />
        </v-col>
      </v-row>
      <v-row>
        <v-col class="pa-0">
          <NotYetAddArticle />
        </v-col>
      </v-row>
    </v-col>

    <v-col
      cols="12"
      md="3"
      :class="dynamicPosition"
      style="right:0;"
      class="mt-md-4 pa-0 commit-now"
    >
      <CommitNow />
    </v-col>

    <v-row :justify="dynamicJustify" class="px-3 px-lg-16 px-md-8 px-xl-16">
      <v-col class="mainslot" cols="12" md="6">
        <div class="mainpage">
          <FollowerMap class="mb-4 my-md-6" />
          <MyState @add-commit="addCommit" />
          <AllArticle class="my-4" :key="'mainArticle' + boardRefresh" />
        </div>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
import AllArticle from '../../components/index/main/AllArticle';
import FollowerMap from '../../components/index/main/FollowerMap';
import MyState from '../../components/index/main/MyState';
import CommitNow from '../../components/index/main/CommitNow';
import NotYetAddArticle from '../../components/index/main/NotYetAddArticle';
import ProfileSummary from '../../components/index/main/ProfileSummary';
import { mapGetters } from 'vuex';

export default {
  components: {
    AllArticle,
    FollowerMap,
    MyState,
    CommitNow,
    NotYetAddArticle,
    ProfileSummary,
  },
  computed: {
    ...mapGetters({ boardRefresh: ['getBoardRefresh'] }),
    dynamicPosition() {
      switch (this.$vuetify.breakpoint.name) {
        case 'xs':
          return 'overflow-sm-style';
        case 'sm':
          return 'overflow-sm-style';
        case 'md':
          return 'overflow-style';
        case 'lg':
          return 'overflow-style';
        case 'xl':
          return 'overflow-style';
      }
      return '';
    },
    dynamicJustify() {
      switch (this.$vuetify.breakpoint.name) {
        case 'xs':
          return '';
        case 'sm':
          return '';
        case 'md':
          return 'center';
        case 'lg':
          return 'center';
        case 'xl':
          return 'center';
      }
      return '';
    },
  },
  methods: {
    addCommit() {
      this.$emit('add-commit');
    },
  },
};
</script>

<style scoped>
.overflow-style {
  position: fixed;
  overflow-y: scroll;
  max-height: calc(100vh - 64px);
}
.overflow-sm-style {
  overflow: hidden;
}
.commit-now {
  -ms-overflow-style: none;
}
.commit-now::-webkit-scrollbar {
  display: none;
}
</style>
