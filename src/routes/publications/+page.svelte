<script lang="ts">
    import Publication from "$lib/publication.svelte";

    const publications = [
        {
            title: "Improving neural network accuracy by concurrently training with a twin network",
            date: "Apr 2025",
            link: "https://openreview.net/forum?id=TEmE9PSC65",
            published: "ICLR'25",
            image: "people/benjamin.jpg",
            description: "We show the applicability of twin network augmentation on convolutional neural networks"
        },
        {
            title: "Compositionality unlocks deep interpretable models",
            date: "Dec 2024",
            published: "AAAI CoLoRAI workshop",
            image: "people/thomas.jpg",
            description: "Introducing a global SVD-like algorithm for multi-linear models.",
        },
        {
            title: "Bilinear MLPs enable weight-based mechanistic interpretability",
            date: "Oct 2024",
            published: "ICLR'25",
            link: "https://tdooms.github.io/research/bilinear",
            image: "people/thomas.jpg",
            description: "Using bilinear MLPs to reverse-engineer shallow MNIST and Tiny Stories models from their weights.",
        },
        {
            title: "Twin Network Augmentation",
            link: "https://arxiv.org/pdf/2409.15849",
            published: "arXiv",
            date: "Sep 2024",
            image: "people/benjamin.jpg",
            description: "A Novel Training Strategy for Improved Spiking Neural Networks and Efficient Weight Quantization."
        },
        {
            title: "Weight-based Decomposition: A Case for Bilinear MLPs",
            date: "Jun 2024",
            published: "ICML MI workshop",
            description: "Introducing bilinear MLPs as a new approach to weight-based interpretability.",
            image: "people/thomas.jpg",
            link: "https://tdooms.github.io/research/bilinear"
        },
        {
            title: "Tokenized SAEs: Disentangling SAE Reconstructions",
            date: "Jun 2024",
            published: "ICML MI workshop",
            description: "We propose using a per-token bias in SAEs to separate token reconstructions from interesting, semantic features.",
            image: "people/thomas.jpg",
            link: "https://tdooms.github.io/research/tokenized"
        },
        {
            title: "The Trifecta: Three techniques for deeper Forward-Forward networks",
            date: "Nov 2023",
            published: "TMLR",
            description: "Three techniques to significantly improve the Forward-Forward algorithm. We achieve 84% on CIFAR-10.",
            image: "people/thomas.jpg",
            link: "https://tdooms.github.io/research/trifecta"
        },
  ]
</script>


{#each publications as publication}
    <Publication {...publication} />
{/each}
