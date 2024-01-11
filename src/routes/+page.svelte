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
  >
    <svg
      xmlns="http://www.w3.org/2000/svg"
      width="18"
      height="18"
      viewBox="0 0 24 24"
      ><g fill="none"
        ><path
          d="M24 0v24H0V0zM12.593 23.258l-.011.002l-.071.035l-.02.004l-.014-.004l-.071-.035c-.01-.004-.019-.001-.024.005l-.004.01l-.017.428l.005.02l.01.013l.104.074l.015.004l.012-.004l.104-.074l.012-.016l.004-.017l-.017-.427c-.002-.01-.009-.017-.017-.018m.265-.113l-.013.002l-.185.093l-.01.01l-.003.011l.018.43l.005.012l.008.007l.201.093c.012.004.023 0 .029-.008l.004-.014l-.034-.614c-.003-.012-.01-.02-.02-.022m-.715.002a.023.023 0 0 0-.027.006l-.006.014l-.034.614c0 .012.007.02.017.024l.015-.002l.201-.093l.01-.008l.004-.011l.017-.43l-.003-.012l-.01-.01z"
        ></path><path
          fill="currentColor"
          d="m2.068 5.482l8.875 8.876a1.5 1.5 0 0 0 2.008.103l.114-.103l8.869-8.87c.029.11.048.222.058.337L22 6v12a2 2 0 0 1-1.85 1.995L20 20H4a2 2 0 0 1-1.995-1.85L2 18V6c0-.12.01-.236.03-.35zM20 4c.121 0 .24.01.355.031l.17.039l-8.52 8.52l-8.523-8.522c.11-.03.224-.05.34-.06L4 4z"
        ></path></g
      ></svg
    >
    <span class="ml-1">E-Mail</span></a
  >
  <button
    type="button"
    class="btn btn-sm variant-filled-surface mt-5 mx-1"
    on:click="{show}"
  >
    <span class="text-warning-500">
      <svg
        xmlns="http://www.w3.org/2000/svg"
        width="18"
        height="18"
        viewBox="0 0 256 256"
        ><path
          fill="currentColor"
          d="M160 16a80.07 80.07 0 0 0-76.09 104.78l-57.57 57.56A8 8 0 0 0 24 184v40a8 8 0 0 0 8 8h40a8 8 0 0 0 8-8v-16h16a8 8 0 0 0 8-8v-16h16a8 8 0 0 0 5.66-2.34l9.56-9.57A80 80 0 1 0 160 16m20 76a16 16 0 1 1 16-16a16 16 0 0 1-16 16"
        ></path></svg
      >
    </span>
    <span class="ml-1">PGP</span>
  </button>
</div>
