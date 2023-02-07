<script>
  import "@skeletonlabs/skeleton/themes/theme-crimson.css";
  import "@skeletonlabs/skeleton/styles/all.css";
  import "../app.postcss";
  import { LightSwitch } from "@skeletonlabs/skeleton";
  import { AppShell, AppBar } from "@skeletonlabs/skeleton";
</script>

<!-- App Shell -->
<AppShell slotSidebarLeft="bg-surface-500/5 w-56 p-4">
  <svelte:fragment slot="header">
    <!-- App Bar -->
    <AppBar>
      <svelte:fragment slot="lead">
        <a href="#MainContent"><strong class="text-xs md:text-xl">АДМИНИСТРАЦИЯ МО <br class="md:hidden"/>"СЕЛО ТЛЯДАЛ"</strong></a>
      </svelte:fragment>
      <svelte:fragment slot="trail">
        <a class="btn btn-sm variant-ghost-surface" href="#History">История</a>
        <a
          class="btn btn-sm variant-ghost-surface"
          href="#Contacts">Контакты</a
        >
        <a class="hidden underline sm:flex" href="tel:+7903499238">+7 (903) 499-02-38</a>
        <div class="hidden sm:flex">
          <LightSwitch />
        </div>
      </svelte:fragment>
    </AppBar>
  </svelte:fragment>
  <!-- Page Route Content -->
  <slot />
</AppShell>
