<script>
  import Icon from "@iconify/svelte";
  import { CodeBlock, modalStore } from "@skeletonlabs/skeleton";
  const show = () => {
    modalStore.trigger({
      type: "component",
      component: "pgp",
    });
  };
</script>

<div class="text-center mt-5">
  <h3 class="h3">Yannik Olmo Hake</h3>

  <a
    href="mailto:yannik.hake@gmail.com"
    class="btn btn-sm variant-filled-surface mt-5"
    ><Icon icon="mingcute:mail-fill" class="inline text-lg" />
    <span class="ml-1">E-Mail</span></a
  >
  <button
    type="button"
    class="btn btn-sm variant-filled-surface mt-5 mx-1"
    on:click="{show}"
  >
    <Icon icon="ph:key-fill" class="inline text-warning-500 text-lg" />
    <span class="ml-1">PGP</span>
  </button>
</div>
