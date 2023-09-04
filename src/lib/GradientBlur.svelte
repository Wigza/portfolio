<style>
    :root {
        --dark: 15, 23, 42,;
        --light: 0, 0, 0,;
    }
    @media (max-width: 640px) {
        .gradient-blur {
            display: none;
        }
    }
    .gradient-blur > div,
    .gradient-blur::before,
    .gradient-blur::after {
        position: absolute;
        inset: 0;
    }
    .gradient-blur::before {
        content: "";
        z-index: 1;
        backdrop-filter: blur(0.5px);
        mask: linear-gradient(
            to bottom,
            rgba(var(--light) 0) 0%,
            rgba(var(--light) 1) 12.5%,
            rgba(var(--light) 1) 25%,
            rgba(var(--light) 0) 37.5%
        );
    }
    .gradient-blur > div:nth-of-type(1) {
        z-index: 2;
        backdrop-filter: blur(1px);
        mask: linear-gradient(
            to bottom,
            rgba(var(--light) 0) 12.5%,
            rgba(var(--light) 1) 25%,
            rgba(var(--light) 1) 37.5%,
            rgba(var(--light) 0) 50%
        );
    }
    .gradient-blur > div:nth-of-type(2) {
        z-index: 3;
        backdrop-filter: blur(2px);
        mask: linear-gradient(
            to bottom,
            rgba(var(--light) 0) 25%,
            rgba(var(--light) 1) 37.5%,
            rgba(var(--light) 1) 50%,
            rgba(var(--light) 0) 62.5%
        );
    }
    .gradient-blur > div:nth-of-type(3) {
        z-index: 4;
        backdrop-filter: blur(4px);
        mask: linear-gradient(
            to bottom,
            rgba(var(--light) 0) 37.5%,
            rgba(var(--light) 1) 50%,
            rgba(var(--light) 1) 62.5%,
            rgba(var(--light) 0) 75%
        );
    }
    .gradient-blur > div:nth-of-type(4) {
        z-index: 5;
        backdrop-filter: blur(8px);
        mask: linear-gradient(
            to bottom,
            rgba(var(--light) 0) 50%,
            rgba(var(--light) 1) 62.5%,
            rgba(var(--light) 1) 75%,
            rgba(var(--light) 0) 87.5%
        );
    }
    .gradient-blur > div:nth-of-type(5) {
        z-index: 6;
        backdrop-filter: blur(16px);
        mask: linear-gradient(
            to bottom,
            rgba(var(--light) 0) 62.5%,
            rgba(var(--light) 1) 75%,
            rgba(var(--light) 1) 87.5%,
            rgba(var(--light) 0) 100%
        );
    }
    .gradient-blur > div:nth-of-type(6) {
        z-index: 7;
        backdrop-filter: blur(32px);
        mask: linear-gradient(
            to bottom,
            rgba(var(--light) 0) 75%,
            rgba(var(--light) 1) 87.5%,
            rgba(var(--light) 1) 100%
        );
    }
    .gradient-blur::after {
        content: "";
        z-index: 8;
        backdrop-filter: blur(64px);
        mask: linear-gradient(
            to bottom,
            rgba(var(--light) 0) 87.5%,
            rgba(var(--light) 1) 100%
        );
    }
    /* dark */
    .dark .gradient-blur::before {
        content: "";
        z-index: 1;
        backdrop-filter: blur(0.5px);
        mask: linear-gradient(
            to bottom,
            rgba(var(--dark) 0) 0%,
            rgba(var(--dark) 1) 12.5%,
            rgba(var(--dark) 1) 25%,
            rgba(var(--dark) 0) 37.5%
        );
    }
    .dark .gradient-blur > div:nth-of-type(1) {
        z-index: 2;
        backdrop-filter: blur(1px);
        mask: linear-gradient(
            to bottom,
            rgba(var(--dark) 0) 12.5%,
            rgba(var(--dark) 1) 25%,
            rgba(var(--dark) 1) 37.5%,
            rgba(var(--dark) 0) 50%
        );
    }
    .dark .gradient-blur > div:nth-of-type(2) {
        z-index: 3;
        backdrop-filter: blur(2px);
        mask: linear-gradient(
            to bottom,
            rgba(var(--dark) 0) 25%,
            rgba(var(--dark) 1) 37.5%,
            rgba(var(--dark) 1) 50%,
            rgba(var(--dark) 0) 62.5%
        );
    }
    .dark .gradient-blur > div:nth-of-type(3) {
        z-index: 4;
        backdrop-filter: blur(4px);
        mask: linear-gradient(
            to bottom,
            rgba(var(--dark) 0) 37.5%,
            rgba(var(--dark) 1) 50%,
            rgba(var(--dark) 1) 62.5%,
            rgba(var(--dark) 0) 75%
        );
    }
    .dark .gradient-blur > div:nth-of-type(4) {
        z-index: 5;
        backdrop-filter: blur(8px);
        mask: linear-gradient(
            to bottom,
            rgba(var(--dark) 0) 50%,
            rgba(var(--dark) 1) 62.5%,
            rgba(var(--dark) 1) 75%,
            rgba(var(--dark) 0) 87.5%
        );
    }
    .dark .gradient-blur > div:nth-of-type(5) {
        z-index: 6;
        backdrop-filter: blur(16px);
        mask: linear-gradient(
            to bottom,
            rgba(var(--dark) 0) 62.5%,
            rgba(var(--dark) 1) 75%,
            rgba(var(--dark) 1) 87.5%,
            rgba(var(--dark) 0) 100%
        );
    }
    .dark .gradient-blur > div:nth-of-type(6) {
        z-index: 7;
        backdrop-filter: blur(32px);
        mask: linear-gradient(
            to bottom,
            rgba(var(--dark) 0) 75%,
            rgba(var(--dark) 1) 87.5%,
            rgba(var(--dark) 1) 100%
        );
    }
    .dark .gradient-blur::after {
        content: "";
        z-index: 8;
        backdrop-filter: blur(64px);
        mask: linear-gradient(
            to bottom,
            rgba(var(--dark) 0) 87.5%,
            rgba(var(--dark) 1) 100%
        );
    }
</style>

<div class="rotate-180 gradient-blur fixed top-0 z-20 w-full h-28">
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
</div>