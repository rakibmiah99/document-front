<script setup lang="ts">
const route = useRoute()

const links = [{
  label: 'Profile',
}, {
  label: 'Installation',
  to: '/'
}, {
  label: 'Horizontal Navigation',
  to: ``
}, {
  label: 'Command Palette',
  to: '/components/command-palette'
}]

const ui ={
  wrapper: 'relative w-full flex items-center justify-between',
  container: 'flex items-center min-w-0 ',
  inner: 'min-w-0 ',
  base: 'group text-white relative w-full flex items-center ',
  before: 'before:absolute before:hover:bg-violet-500 before:hover:rounded-none before:inset-x-0 before:inset-y-2 before:inset-px before:rounded-md',
  after: 'after:absolute  after:bottom-0 after:inset-x-2.5 after:block after:h-[2px] after:mt-2 bg-none',
  active: 'text-white border-0 bg-violet-500 rounded-none after:bg-indigo-0',
  inactive: 'text-white  dark:text-gray-400 hover:text-gray-300 dark:hover:text-white',
  label: 'truncate relative ',
  icon: {
    base: 'flex-shrink-0 w-5 h-5 relative',
    active: 'text-gray-700 dark:text-gray-200',
    inactive: 'text-gray-400 dark:text-gray-500 group-hover:text-gray-700 dark:group-hover:text-gray-200',
  },
  avatar: {
    base: 'flex-shrink-0',
    size: '2xs',
  },
  badge: {
    base: 'flex-shrink-0 ml-auto relative rounded',
    color: 'gray',
    variant: 'solid',
    size: 'xs',
  },
}


</script>

<template>
    <div class="bg-slate-900">
        <UContainer>
            <UHorizontalNavigation :ui="ui" :links="links"  />
        </UContainer>
    </div>
  
</template>

