<template>
  <q-layout ref="layout" view="hHr LpR Fff">

  <q-toolbar slot="header" color="deep-purple-13">
    <q-btn flat @click="$refs.layout.toggleLeft()">
      <q-icon name="menu" />
    </q-btn>
    <div class="q-toolbar-title">
      <h5>.dot</h5>
    </div>
  </q-toolbar>

  <div class="layout-padding justify-center">
    <q-list highlight>
      <q-list-header>To do today</q-list-header>
      <q-item >
        <q-item-side><q-checkbox v-model="checked" color="teal" /></q-item-side>
        <q-item-main inline >
          <q-item-tile label>Quasar enthusiastasssssssssssssssssd ssssssssssssssssss ssssssssssssssssss   Doe</q-item-tile>
          <q-item-tile sublabel>
            <q-item-tile icon="date range"/>
            sdfsdfsdf
          </q-item-tile>
        </q-item-main>
        <q-item-side right>
          <q-item-tile>
            <q-btn flat>
              <q-item-tile icon="delete" color="grey" />
            </q-btn>
          </q-item-tile>
        </q-item-side>
      </q-item>
      <q-item>
        <q-item-side>
          <q-item-tile avatar>
            <img src="~assets/boy-avatar.png" />
          </q-item-tile>
        </q-item-side>
        <q-item-main label="John Doe" sublabel="Quasar enthusiast" />
        <q-item-side right icon="chat_bubble" />
      </q-item>
      <q-item-separator />
      <q-list-header>You got done</q-list-header>
      <q-item>
        <q-item-side avatar="/statics/guy-avatar.png" />
        <q-item-main label="Jack Doe" />
      </q-item>
    </q-list>
  </div>

  <div slot="left">
    <q-side-link item to="/test-layout" exact>
      <q-item-main label="About" />
    </q-side-link>
    <q-side-link item to="/test-layout/toolbar">
      <q-item-main label="Toolbar" />
    </q-side-link>
  </div>
</q-layout>
</template>

<script>
import {
  QCollapsble,
  QCheckbox,
  QCard,
  QCardTitle,
  QCardSeparator,
  QCardMain,
  QSideLink,
  QLayout,
  QToolbar,
  QToolbarTitle,
  QBtn,
  QIcon,
  QList,
  QListHeader,
  QItem,
  QItemSide,
  QItemMain,
  QItemTile,
  QItemSeparator
} from 'quasar'

export default {
  name: 'index',
  components: {
    QCollapsble,
    QCheckbox,
    QCard,
    QCardTitle,
    QCardSeparator,
    QCardMain,
    QSideLink,
    QLayout,
    QToolbar,
    QToolbarTitle,
    QBtn,
    QIcon,
    QList,
    QListHeader,
    QItem,
    QItemSide,
    QItemMain,
    QItemTile,
    QItemSeparator
  },
  data() {
    return {
      items: [
        {
          title: 'Card title',
          content: 'Content content',
          date: new Date()
        },
        {
          title: 'Card title',
          content: 'Content content',
          date: new Date()
        },
        {
          title: 'Card title',
          content: 'Content content',
          date: new Date()
        },
        {
          title: 'Card title',
          content: 'Content content',
          date: new Date()
        },
        {
          title: 'Card title',
          content: 'Content content',
          date: new Date()
        }
      ],
      checked: []
    }
  }
}
</script>

<style>
  .q-toolbar-title h5 {
    font-weight: 300;
  }
</style>







