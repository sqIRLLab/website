<script lang="ts">
    import Event from "$lib/event.svelte";

  const events = [
    {
        title: "Talk @ VisAPP'24",
        date: "27 Feb 2025",
        link: "publications/_example",
        image: "people/benjamin.jpg",
        description: "Recognizing actions in high-resolution low-framerate videos: a feasibility study in the construction sector.",
    },
    {
        title: "Talk @ Flanders AI Day",
        date: "14 Oct 2024",
        link: "https://docs.google.com/presentation/d/1PdcHm0bgwIu3yhy6oWkwL1-fDGTPzTiyUilydognLlw/edit?usp=sharing",
        image: "people/thomas.jpg",
        description: "A swift introduction to weight-based interpretability.",
    },
  ]
</script>


{#each events as event}
    <Event {...event} />
{/each}
