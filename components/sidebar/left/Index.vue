<template>
  <aside class="flex flex-col h-screen gap-4">
    <nuxt-link to="/" class="p-2">
      <Logo />
    </nuxt-link>
    <div class="mt-2 space-y-2">
      <SidebarLeftTab active>
        <template v-slot:icon>
          <HomeIcon />
        </template>
        <template v-slot:title>
          Home
        </template>
      </SidebarLeftTab>
      <SidebarLeftTab >
        <template v-slot:icon>
          <HashtagIcon/>
        </template>
        <template v-slot:title>
          Explore
        </template>
      </SidebarLeftTab>
      <SidebarLeftTab >
        <template v-slot:icon>
          <BellIcon />
        </template>
        <template v-slot:title>
          Notifications
        </template>
      </SidebarLeftTab>
      <SidebarLeftTab >
        <template v-slot:icon>
          <InboxIcon />
        </template>
        <template v-slot:title>
          Messages
        </template>
      </SidebarLeftTab>
      <SidebarLeftTab >
        <template v-slot:icon>
          <BookmarkIcon />
        </template>
        <template v-slot:title>
          Bookmarks
        </template>
      </SidebarLeftTab>
      <SidebarLeftTab >
        <template v-slot:icon>
          <DocumentTextIcon />
        </template>
        <template v-slot:title>
          Lists
        </template>
      </SidebarLeftTab>
      <SidebarLeftTab >
        <template v-slot:icon>
          <UserIcon/>
        </template>
        <template v-slot:title>
          Profile
        </template>
      </SidebarLeftTab>
      <SidebarLeftTab >
        <template v-slot:icon>
          <EllipsisHorizontalCircleIcon/>
        </template>
        <template v-slot:title>
          More
        </template>
      </SidebarLeftTab>
    </div>
  </aside>
</template>

<script setup>
import { HomeIcon } from '@heroicons/vue/24/solid';
import { BellIcon, UserIcon, BookmarkIcon, DocumentTextIcon, HashtagIcon, EllipsisHorizontalCircleIcon, InboxIcon } from '@heroicons/vue/24/outline'
</script>