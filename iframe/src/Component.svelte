<script>
  import { getContext } from "svelte"

  export let text

  const { styleable } = getContext("sdk")
  const component = getContext("component")
</script>

<div use:styleable={$component.styles}>
  <iframe src="https://www.example.com" width="600" height="400" style="border:1px solid black;">
        Seu navegador não suporta iFrames.
    </iframe>
</div>
