<template>
    <footer class="main-footer">
        <div class="container">
            <div class="columns">
                <div class="column">
                    <a
                        href="https://creativecommons.org"
                        class="main-logo margin-bottom-bigger has-text-white"
                    >
                        <svg
                            xmlns="http://www.w3.org/2000/svg"
                            preserveAspectRatio="xMidYMid meet"
                            viewBox="0 0 304 73"
                        >
                            <use href="~@creativecommons/vocabulary/assets/logos/cc/logomark.svg#logomark" />
                        </svg>
                    </a>
                    <address class="margin-bottom-normal">
                        <span class="is-block">Creative Commons</span>
                        <span>PO Box 1866, Mountain View CA 94042</span>
                    </address>
                    <a
                        href="mailto:info@creativecommons.org"
                        class="mail is-block"
                    >
                        info@creativecommons.org
                    </a>
                    <a
                        href="tel://+1-415-429-6753"
                        class="phone"
                    >+1-415-429-6753</a>

                    <div class="margin-vertical-large">
                        <a
                            href="https://www.instagram.com/creativecommons"
                            class="social has-text-white"
                            target="_blank"
                            rel="noopener"
                        >
                            <i class="icon instagram margin-right-small is-size-4" />
                        </a>
                        <a
                            href="https://www.twitter.com/creativecommons"
                            class="social has-text-white"
                            target="_blank"
                            rel="noopener"
                        >
                            <i class="icon twitter margin-right-small is-size-4" />
                        </a>
                        <a
                            href="https://www.facebook.com/creativecommons"
                            class="social has-text-white"
                            target="_blank"
                            rel="noopener"
                        >
                            <i class="icon facebook margin-right-small is-size-4" />
                        </a>
                        <a
                            href="https://www.linkedin.com/company/creative-commons/"
                            class="social has-text-white"
                            target="_blank"
                            rel="noopener"
                        >
                            <i class="icon linkedin margin-right-small is-size-4" />
                        </a>
                    </div>
                </div>
                <div class="column">
                    <nav class="footer-navigation">
                        <ul class="menu">
                            <li>
                                <a
                                    class="menu-item"
                                    href="https://docs.google.com/forms/d/e/1FAIpQLSfF7MCKxlPsPuMn17v_sLYWMkxBkudQSPXCXoJKjh5GCtx63g/viewform"
                                >Feedback</a>
                            </li>
                        </ul>
                    </nav>
                    <div class="attribution margin-top-bigger">
                        <p class="caption">
                            Except where otherwise
                            <a
                                href="https://creativecommons.org/policies#license"
                                target="_blank"
                                rel="noopener"
                            >noted</a>,
                            content on this site is licensed under the
                            <a
                                href="https://creativecommons.org/licenses/by/4.0/"
                                target="_blank"
                                rel="noopener"
                            >
                                Creative Commons Attribution 4.0 International license
                            </a>.
                            <a
                                href="https://fontawesome.com/"
                                target="_blank"
                                rel="noopener"
                                class="has-text-white"
                            >
                                Icons by Font Awesome.
                            </a>
                        </p>

                        <div class="margin-top-smaller">
                            <i class="icon cc-logo margin-right-small is-size-4 is-color-white" />
                            <i class="icon cc-by margin-right-small is-size-4 is-color-white" />
                        </div>
                    </div>
                </div>
                <div class="column">
                    <aside class="donate-section">
                        <h5>{{ $t('footer.donation.header') }}                        </h5>
                        <p>{{ $t('footer.donation.call') }}</p>
                        <a
                            class="button small donate"
                            href="http://creativecommons.org/donate"
                        >
                            <i class="icon cc-letterheart margin-right-small is-size-5 padding-top-smaller" />
                            Donate now
                        </a>
                    </aside>
                </div>
            </div>
        </div>
    </footer>
</template>

<script>
export default {
    name: 'FooterSection'
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
    .donate, .social {
        &:hover {
            text-decoration: none;
        }
    }

    .icon {
        vertical-align: middle;
    }
    @media screen and (min-width: 1023px) {
        // All columns are set the same width on 'tablet'-sized screen
        // Half-sized middle column makes the last column too small for
        // the 'Donate' button and breaks the layout
        .column:nth-child(2) {
            flex: none;
            width: 50%;
        }
    }
</style>
