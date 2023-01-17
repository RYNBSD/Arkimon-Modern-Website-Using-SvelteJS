<script>
    import Fa from "svelte-fa";
    import { faArrowRight, faAngleDown } from "@fortawesome/free-solid-svg-icons";

    import { faq } from "../constants";
    const array = ['', '', '', ''];
</script>

<section class="arkimon__faq">
    <div class="arkimon__faq-container">
        <div class="arkimon__faq-container_left f-center">
            <div class="arkimon__faq-container_left-elements f-center">
                {#each array as arr, index (index)}
                    <div class="arkimon__faq-container_left-elements_element">
                        <div class="arkimon__faq-container_left-elements_element-title f-center">
                            <h2>When i  need to contact with you?.</h2>
                            <Fa icon={faAngleDown} size="2x" primaryColor="#4E4E4E" />
                        </div>
                        <div class="arkimon__faq-container_left-elements_element-content">
                            <p>If you are ipsum dolor sit amet, consectetur adipiscing elit. Enim, nisi eget egestas proin. Diam bibendum facilisi risus scelerisque tellus bibendum tristique. Sit augue id nibh feugiat dui. Ipsum tortor integer suspendisse arcu, maecenas lacus. Rhoncus ac.</p>
                        </div>
                    </div>
                {/each}
            </div>
            <div class="arkimon__faq-container_left-btn">
                <button type="button" class="f-center">
                    More Question?
                    <Fa icon={faArrowRight} />
                </button>
            </div>
        </div>
        <div class="arkimon__faq-container_right">
            <img src={faq} alt="faq">
        </div>
    </div>
</section>