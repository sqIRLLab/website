<script lang="ts">
  import Person from "$lib/person.svelte";

  const people = [
    {
          name: "Jose Oramas",
          status: "Professor",
          specialty: "Model Interpretability and Explainability",
          image: "people/jose.png",
          link: "https://webserver.idlab.uantwerpen.be/~joramasmogrovejo/"
    },
    {
        name: "Thomas Dooms",
        status: "PhD student",
        specialty: "Weight-based interpretability",
        image: "people/thomas.jpg",
        link: "https://tdooms.github.io/"
    },
    {
      name: "Benjamin Versmissen",
      status: "PhD student",
      specialty: "Representation learning with a focus on the Lottery Ticket Hypothesis",
      image: "people/benjamin.jpg",
      link: "https://scholar.google.com/citations?user=pfgVNMUAAAAJ&hl=en"
    },
    {
      name: "Fabian Denoodt",
      status: "PhD student",
      specialty: "Trustworthy and reliable learning",
      image: "people/fabian.jpg",
      link: "https://fdenoodt.github.io/"
    },
    {
      name: "Saja Tawalbeh",
      status: "PhD student",
      specialty: "Explainable Artificial Intelligence",
      image: "people/saja.png",
      link: "https://stawalbeh.github.io/STawalbeh/"
    },
  ]
</script>



{#each people as person}
  <Person {...person} />
{/each}
