<script lang="ts">
  import { dictionary } from "../scripts/localization";
  import { SLOW_NETWORK, USER } from "../store";
</script>

{#if SLOW_NETWORK}
  <div class="slow-network">
    {@html dictionary[$USER.language].settings.degradedNetworkPerformance}
  </div>
{/if}