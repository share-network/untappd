<script>
  import "../app.postcss";
  import { dev } from "$app/environment";
</script>

<slot />

{#if !dev}
<script defer src='https://static.cloudflareinsights.com/beacon.min.js' data-cf-beacon='{"{"}"token": "6e633c6ed03340bb93e852a2ca928ea4"{"}"}'></script>
{/if}
